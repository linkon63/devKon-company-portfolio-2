<template>
    <div class="flex flex-col gap-4 justify-center items-center w-[433.33px] h-[408px] bg-[#FFFFFF] rounded-[30px] p-8 relative overflow-hidden group">
        <div class="img">
            <img :src="getImgUrl()" />
        </div>
        <div class="title text-[#212121] text-xl md:text-2xl lg:text-3xl">
            <h3>{{ props.title }}</h3>
        </div>
        <div class="description text-center text-[#6E6E73] font-lg md:font-xl lg:font-2xl leading-6 w-3/4">
            <p>{{ props.description }}</p>
        </div>
        <div class="p-16 hover-div flex flex-col gap-4 justify-center items-center absolute bg-[#F7F7FF] w-[433.33px] h-[408px] rounded-[30px] transform translate-y-full transition ease-in-out duration-[800ms] group-hover:translate-y-0">
            <div class="title  text-[#212121] text-xl md:text-2xl lg:text-3xl">
                <h3>{{ props.hoverTitle }}</h3>
            </div>
            <div class="description text-center text-[#6E6E73] font-lg md:font-xl lg:font-2xl leading-6 w-3/4">
                <p>{{ props.hoverDescription }}</p>
            </div>
        </div>
    </div>
</template>


<script setup>

const props = defineProps({
    logo: String,
    title: String,
    description: String,
    hoverTitle: String,
    hoverDescription: String,
});

const getImgUrl = () => {
    return '/working-with-us/'+props.logo;
}

</script>

