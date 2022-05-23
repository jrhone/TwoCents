<script>
  import { createEventDispatcher } from 'svelte';
  const dispatch = createEventDispatcher();

  let name;
</script>

<div class="box">
  <img src="/profile.svg" class="w-8 h-8" alt="create icon"/>
  <input 
    class="create" 
    bind:value={name} 
    on:keyup={e => e.key==='Enter' && dispatch("submit", name)}
    placeholder="Create a post" 
    type="text"/>
  <div class="flex">
    <img src="/media.svg" class="w-4 h-4 mx-2.5" alt="media icon"/>
    <img src="/link.svg" class="w-4 h-4 mx-2.5" alt="link icon"/>
  </div>
</div>

<style>
  .box {
    @apply flex space-x-2 items-center;
    @apply px-4 py-2;
    background: #191C25;
    border: 1px solid #1D2939;
    border-radius: 8px;
  }

  input {
    background: #0E1116;
    box-shadow: 0px 1px 2px rgba(16, 24, 40, 0.05);
    border-radius: 4px;
    @apply px-3.5 py-2.5;
    @apply w-full;

    font-family: 'Source Sans Pro';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    color: #98A2B3;
  }
</style>