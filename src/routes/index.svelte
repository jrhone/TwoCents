<script>
  import Create from '../components/Create.svelte';
  import Filter from '../components/Filter.svelte';
  import Leaderboard from '../components/Leaderboard.svelte';
  import Overview from '../components/Overview.svelte';
  import Post from '../components/Post.svelte';
  import Summary from '../components/Summary.svelte';

  const createPost = ({ detail }) => {
    posts = [...posts, {
      name: detail,
      image: '/default_post.png',
    }];
  };

  let posts = [];
</script>


<div class="my-4">
  <Summary/>
</div>
<div class="flex flex-row space-x-8">
  <div class="w-[612px] space-y-4">
    <Create on:submit="{createPost}"/>
    <Filter />

    {#each posts as post}
      <Post name={post.name} image={post.image} />
    {/each}
  </div>
  <div class="w-[354px] space-y-4">
    <Overview />
    <Leaderboard />
  </div>
</div>


<style>
</style>