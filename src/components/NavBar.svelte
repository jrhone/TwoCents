<div class="navbar">
  <img src="/logo.svg" class="w-6 h-6 lg:mr-40" alt="logo"/>
  <input class="search" placeholder="Search 2Cents" type="text"/>
  <div class="flex space-x-8 items-center">
    <div class="post">New post</div>
    <img src="/bell.svg" class="w-4 h-4" alt="bell icon"/>
    <img src="/profile.svg" class="w-6 h-6" alt="profile icon"/>
  </div>
</div>

<style>
  .navbar {
    @apply flex justify-between;
    @apply px-10 py-2;
    @apply items-center;
  }

  .post {
    background: #5E77FF;
    box-shadow: 0px 1px 2px rgba(16, 24, 40, 0.05);
    border-radius: 4px;
    padding: 8px 14px;

    font-family: 'Source Sans Pro';
    font-style: normal;
    font-weight: 600;
    font-size: 14px;
    line-height: 20px;
    color: #1D2939;
    white-space: nowrap;
  }

  .search {
    @apply h-11;
    @apply w-[484px];
    @apply px-3 py-2;

    background: #0E1116;
    border: 1px solid #191C25;
    box-shadow: 0px 1px 2px rgba(16, 24, 40, 0.05);
    border-radius: 4px;

    font-family: 'Source Sans Pro';
    font-style: normal;
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    color: #98A2B3;
  }
</style>
