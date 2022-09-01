<script setup></script>

<template>
  <main>
 <h1 class ="title">Vue Grocery List</h1>
 <form class="newGroceryForm">
        <input 
            id="newGrocery" 
            autocomplete="off"
            type="text" 
            placeholder="Add an item to your list"/>
        <button id="addBtn" type = "submit"> Add</button>
    </form>
    <form>
      <ul>
        <li>Tortilla</li>
      </ul>
    </form>
</main>
</template>

<style lang="postcss" scoped>
main{
  @apply mt-8 flex flex-col justify-center items-center;

  .title{
    @apply m-2 text-6xl font-light tracking-wider text-accent;
  }
    form{
      @apply mt-8 flex focus-within:ring-8 focus-within:ring-accent focus-within:rounded-lg;
     
      input{
        @apply bg-white text-comment p-2 w-80 text-2xl rounded-l-md outline-none;
      }
      
      button{
        @apply bg-accent text-background p-2 text-2xl font-bold rounded-r-md;
        &:hover{
          @apply bg-foreground;
        }
      }
    }
      ul {
           @apply flex flex-col items-center justify-center rounded-lg bg-accent;
          li{
            @apply bg-white text-background m-2 p-2 w-96 text-center;
            &:hover{
              @apply bg-foreground font-bold cursor-pointer;
            }
      }  
      
  }
}
</style>
