<div class="box">
  <slot />
</div>


<style>
  .box {
    @apply flex-col;
    @apply space-y-4;
    @apply p-4;
    background: #191C25;
    border: 1px solid #1D2939;
    border-radius: 8px;
  }
</style>