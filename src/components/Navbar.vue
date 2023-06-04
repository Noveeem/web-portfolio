<script>
    export default{
        name: "Navbar",
        data() {
            return {
                brand: "../assets/media/icon/sourcecode.svg"
            }
        },
        props: {
            btn: {
                type: String,
                default: "Send me a message"
            }
        }
    }
</script>

<template>
    <nav class="navbar">
        <div class="container mx-auto py-4">
            <div class="flex-1 border-none">
                <img v-bind:src="brand" alt="">
            </div>
            <div class="flex-none sm:block">
                <ul class="menu menu-horizontal px-1 sm:hidden">
                    <li class="font-extralight text-lg"><a href="" class="hover:bg-transparent hover:text-white">Home</a></li>
                    <li class="font-extralight text-lg"><a href="" class="hover:bg-transparent hover:text-white">Skills</a></li>
                    <li class="font-extralight text-lg"><a href="" class="hover:bg-transparent hover:text-white">Experiences</a></li>
                    <li class="font-extralight text-lg"><a href="" class="hover:bg-transparent hover:text-white">Projects</a></li>
                </ul>
                <a href="mailto:carlshemrick00@gmail.com" class="btn w-[200px] btn-outline btn-info" target="_blank">
                    <i class="bi bi-send-fill"></i>{{ btn }}
                </a>
            </div>
        </div>
    </nav>
</template>

<style scoped>

</style>
