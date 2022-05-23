<script>
  import Box from '../components/Box.svelte';

  export let name;
  export let image = "/default_post.png";
</script>


<Box>
  <div class="name mb-4">{ name }</div>
  <img src="{image}" alt="Media"/>
</Box>


<style>
  .name {
    font-family: 'Source Sans Pro';
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    line-height: 28px;
    color: #D0D5DD;
  }
</style>