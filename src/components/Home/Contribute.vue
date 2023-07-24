<script setup>
    const section = 'flex flex-col-reverse md:flex-row items-center justify-between gap-8 text-center md:text-left mt-12'
    const img = 'md:w-[256px] w-[180px]'
    const div = 'flex flex-col justify-between gap-10 w-[50%] items-center md:items-start'
    const h1 = 'font-ms text-violet-600 md:text-3xl lg:text-4xl text-2xl sm:text-4xl font-bold text-center'
    const p = 'text-blue-50 font-pp text-md md:text-2xl'
    const a = 'bg-violet-600 w-[184px] h-[50px] flex flex-row items-center rounded-xl justify-center'

</script>

<template>
    <section :class="section">
        <img src="../../assets/contribution.svg" alt="contribution" :class="img">
        <div :class="div">
            <h1 :class="h1">Contribute</h1>
            <p :class="p">Vivi Bot can be upgraded and become a better service with your help!</p>
            <p :class="p">Adding features to the application’s source code will help Vivi Bot to reach more people and increase its help.</p>
            <a href="https://github.com/daviebatista/vivi-bot" target="_blank" :class="a">
                <p :class="p">Try Out</p>
                <img src="../../assets/button-arrow.svg" alt="right-arrow">
            </a>
        </div>
    </section>
</template>

<style scoped lang="scss">
    section {
        background: rgb(0,0,0);
        background: linear-gradient(0deg, rgba(0,0,0,1) 0%, rgba(0,2,22,1) 50%);        
        padding: 100px 12.361111111111%;
        min-height: 100vh;
    }

    a   {
        transition: 0.3s;

        &:hover {
            filter: brightness(110%);

            p   {
            margin-left: 30px;
            }

            img {
                padding-left: 30px;
            }
        }
    }

    p   {
        transition: 0.3s;
    }

    img {
        transition: 0.3s;
    }

    @media (max-width: 1366px) {
        section {
            padding: 100px 85px;
        }
    }

    @media (max-width: 768px) {
        section {
            padding: 0px 0px;
        }
    }
</style>