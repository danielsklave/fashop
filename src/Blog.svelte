<script>
    import {user, heart} from 'svelte-awesome/icons';
  
      import Icon from 'svelte-awesome';
  
  </script>
<div class="flex flex-col h-full gap-4 bg-[url('https://source.unsplash.com/iIjResyhhW0/400x700')]">
    <div class="mt-auto bg-gray-100 px-8 py-4 grid gap-4 rounded-t-[1.5rem]">
        <div class="flex items-center justify-between"><h2><Icon data="{user}" class="mr-2" />Example User</h2><Icon data="{heart}" class="mr-2 text-pink-500" /></div>
        <small class="mb-1">Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet.</small>
        <div class="flex justify-center gap-6">
            <a href="/#/item" class="flex gap-4"><small class="text-center block">Buy this outfit</small> <small>^</small></a>
        </div>
    </div>
</div>
