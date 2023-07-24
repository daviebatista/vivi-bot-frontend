<script setup>
    const div = 'text-center flex flex-col justify-center lg:gap-24 gap-8'
    const strong = 'text-blue-400 font-normal'
    const strong2 = 'text-blue-400'
    const h1 = 'font-ms text-blue-200 font-bold sm:border-b-2 lg:border-b-4 border-blue-200 px-12 self-center'
    const p = 'text-blue-200 text-xl md:text-4xl font-pp text-center px-0 lg:px-44'
</script>

<template>
    <section>
        <div id="hero" :class="div">
            <h1 :class="h1">What is <strong :class="strong2">Vivi Bot</strong>?</h1>
            <p :class="p">
                <strong :class="strong">Vivi Bot</strong> is an open-source Discord Bot Template <strong :class="strong">integrated with RPG-Gaming Tools</strong>,
                made to help people <strong :class="strong">create their own</strong>
                local applications.
            </p>
        </div>
    </section>
</template>

<style scoped>
    section {
        background: url('../../assets/about-1.jpg') no-repeat;
        background-size: cover;
        min-height: 60vh;
        
    }

    #hero   {
        padding: 100px 12.361111111111%;
    }

    h1  {
        font-size: 48px;
    }

    p   {
        line-height: 50px;
    }

    @media (max-width: 1366px) {
        #hero {
            padding: 120px 85px;
        }
    }

    @media (max-width: 768px) {
        section {
            margin-top: 40px;
        }

        #hero {
            padding: 50px 40px;
        }

        h1  {
            font-size: 28px;
            margin-top: 0px;
        }
        
        p   {
            line-height: 30px;
        }
    }

    @media  (max-width: 610px)  {
        section {
            margin-top: -30px;
        }
    }
</style>