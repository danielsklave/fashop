<script>
let username = ""
let password = ""
let login = false;
let errors = [];

const handleSubmit = () => {
    errors = [];
    if(!username) errors.push("username")
    if(!password) errors.push("password")
    if(!errors.length) login = true;
}

</script>

<form class="mx-8 h-full">
{#if login}
<div class="flex gap-4 items-center mt-8">
    <img src="https://source.unsplash.com/vjUokUWbFOs/400x175" class="w-12 aspect-[1/1] rounded-full object-cover" alt="Post">
    <b>{username}</b>
</div>
<div class="flex flex-col gap-6 mt-8">
    <b>Contact Information</b>
    <b>History</b>
    <b>Promo Codes</b>
    <b>Notifications</b>
    <hr/>
    <b>Privacy Policy</b>
    <b>Terms & Condidions</b>
    <b>Support</b>
</div>
{:else}
    <div class="flex flex-col gap-4 bg-gray-100 mt-16 p-6 rounded-[1rem]">
        <div class="grid gap-2">
            <label>Username</label>
            <input class="border rounded-[1rem] h-10 px-4" class:border-red-500={errors.includes("username")} bind:value={username} required/>
        </div>
        <div class="grid  gap-2">
            <label>Password</label>
            <input class="border rounded-[1rem] h-10 px-4" class:border-red-500={errors.includes("password")}  type="password" bind:value={password} required />
        </div>
        <button type="submit" on:click={handleSubmit} class="mt-3 w-full bg-purple-950 text-white font-bold px-12 py-2 rounded-[1rem]">Login</button>
        <small class="text-center">Don't have an account? <b>Register</b></small>
    </div>
    {/if}
</form>
