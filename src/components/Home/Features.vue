<script setup>
    const section = 'flex flex-col md:flex-row items-center justify-between gap-0 sm:gap-8 text-center md:text-left'
    const div = 'flex flex-col lg:gap-14 gap-6'
    const h1 = 'text-blue-50 font-bold font-ms md:text-3xl lg:text-4xl text-2xl sm:text-4xl'
    const ul = 'flex flex-col lg:gap-8 gap-4 font-pp text-blue-400 md:list-disc text-sm md:text-lg md:ml-5 sm:text-xl'
    const img = 'rounded-2xl mt-8 w-[100%] md:w-[350px] lg:w-[437px]'
</script>

<template>
    <section :class="section">
        <div :class="div">
            <h1 :class="h1">Native Features</h1>
            <ul :class="ul">
                <li>Dice Rollings ('/d[number] + [modifier]);</li>
                <li>Exalted/VTM Dice Rollings (‘/er [amount]’);</li>
                <li>Heads or Tails flip (‘/hot’);</li>
                <li>And more to be added.</li>
            </ul>
        </div>
        <div>
            <img src="../../assets/vivi.gif" alt="vivi-gif" :class="img">
        </div>
    </section>
</template>

<style scoped>
    section {
        background: rgb(0,2,22);
        background: linear-gradient(0deg, rgba(0,2,22,1) 50%, rgba(0,0,0,1) 100%);
        padding: 100px 12.361111111111%;
        min-height: 100vh;
    }

    @media (max-width: 1366px) {
        section {
            padding: 100px 85px;
        }
    }

    @media (max-width: 768px) {
        section {
            padding: 0px 40px;
        }
    }
</style>