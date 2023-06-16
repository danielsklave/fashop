<script>
  import {star} from 'svelte-awesome/icons';

	import Icon from 'svelte-awesome';

</script>


<div class="flex flex-col h-full gap-4">
    <div class="grow w-full relative">
        <img src="https://source.unsplash.com/iIjResyhhW0/400x700" class="h-full aspect-[4/3] rounded-lg object-cover w-2/3 mx-auto" alt="Post"> 
        <div class="absolute right-4 bg-white p-3 bottom-4 rounded-lg grid gap-2 text-center shadow-md">
            <div><b>Size</b></div>
            <div>S</div>
            <div>M</div>
            <div>L</div>
            <div>XL</div>
        </div>
    </div>
    <div class="bg-gray-100 px-8 py-4 grid gap-4 rounded-t-[1.5rem]">
        <div class="flex justify-center gap-8">
            <small class="text-center block">Buy this outfit</small> <small><Icon data={star} class="text-yellow-500" /> 4.5</small>
        </div>
        <h2 class="text-center font-bold">Example Outfit 1</h2>
        <ul class="list grid gap-4">
            <li class="flex bg-white rounded shadow-md">
                <img src="https://images.ctfassets.net/w2dr5qwt1rrm/7myamQzgWasnUNRNcG3WQC/65a7d86a94c8cd75418aca8a156d556a/UMQ90LP1K022027R.jpg?w=3000&h=4000&fit=fill&q=70&fm=jpg" class="aspect-[3/4] w-16 rounded object-cover" alt="Post"> 
                <div class="py-2 px-4 w-full">
                    <div><b>Example shirt 1</b> <div class="float-right">x</div><div>
                    <small>View simmilar</small>
                    <div><b>$60.0</b> <b class="float-right">Example store 1</b><div>
                </div>
            </li>
            <li class="flex bg-white rounded shadow-md">
                <img src="https://xcdn.next.co.uk/COMMON/Items/Default/Default/ItemImages/AltItemShot/315x472/D17761s2.jpg" class="aspect-[3/4] w-16 rounded object-cover" alt="Post"> 
                <div class="py-2 px-4 w-full">
                    <div><b>Example coat 1</b> <div class="float-right">x</div><div>
                    <small>View simmilar</small>
                    <div><b>$100.0</b> <b class="float-right">Used (like new)</b><div>
                </div>
            </li>
            <!-- ... -->
        </ul>
        <div class="flex justify-between items-center">
            $160.0
            <a href="/#/cart" class="btn bg-purple-950 text-white font-bold px-8 py-1 rounded-lg">Add to cart</a>
        </div>
    </div>
</div>
