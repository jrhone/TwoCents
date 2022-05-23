<script>
  import Box from '../components/Box.svelte';
</script>

<Box>
  <div class="title mb-4">
    Leaderboard
  </div>
  <div class="row">
    <div class="row-info">
      <img src="/avatar.svg" class="w-6 h-6 mr-2" alt="avatar"/>
      Username
    </div>
    <div class="row-info">
      15.340 $CEN
    </div>
  </div>
</Box>


<style>
  .title {
    font-family: 'Source Sans Pro';
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 24px;
    color: #F9FAFB;
  }

  .row {
    @apply flex justify-between;
    font-family: 'IBM Plex Mono';
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 18px;
    color: #D0D5DD;
  }

  .row-info {
    @apply flex items-center;
  }
</style>