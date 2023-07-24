<script setup>
import { reactive } from 'vue'
const div1 =
  'flex flex-col md:items-start items-center md:justify-start gap-4 md:gap-8 justify-center'
const div2 = 'text-blue-300 font-pp bg-slate-900 w-full rounded-lg p-2 md:p-4 gap-2 flex flex-col'
const h1 = 'md:text-4xl font-ms text-blue-300 font-bold text-2xl text-center'
const h2 = 'md:text-2xl text-sm font-ms font-bold'

const commands = reactive([
  {
    command: 'List All Commands',
    name: '/commands',
    description: "Gives a list of all the bot's native commands"
  },

  {
    command: 'Heads Or Tails',
    name: '/hot',
    description: 'Flips a coin, resulting in "Heads" or "Tails"'
  },

  {
    command: 'D4',
    name: '/d4 [amount] [modifier]',
    description: 'Rolls D4s on the wished amount with the added modifier'
  },

  {
    command: 'D6',
    name: '/d6 [amount] [modifier]',
    description: 'Rolls D6s on the wished amount with the added modifier'
  },

  {
    command: 'D8',
    name: '/d8 [amount] [modifier]',
    description: 'Rolls D8s on the wished amount with the added modifier'
  },

  {
    command: 'D10',
    name: '/d10 [amount] [modifier]',
    description: 'Rolls D10s on the wished amount with the added modifier'
  },

  {
    command: 'D12',
    name: '/d12 [amount] [modifier]',
    description: 'Rolls D12s on the wished amount with the added modifier'
  },

  {
    command: 'D20',
    name: '/d20 [amount] [modifier]',
    description: 'Rolls D20s on the wished amount with the added modifier'
  },

  {
    command: 'Exalted Roll',
    name: '/er [amount]',
    description:
      'Realizes an Exalted/VampireTM based dice rolling, with the amount of dices chosen by the input'
  }
])
</script>

<template>
  <section>
    <div id="commands" :class="div1">
      <h1 :class="h1">Vivi Bot's Native Commands</h1>
      <div v-for="command of commands" :class="div2">
        <h2 :class="h2">
          {{ command.command }}
        </h2>
        <p class="text-xs">
          <strong>{{ command.name }}</strong> - {{ command.description }}
        </p>
      </div>
    </div>
  </section>
</template>

<style>
#commands {
  background: rgb(0, 0, 0);
  background: linear-gradient(0deg, rgba(0, 0, 0, 1) 0%, rgba(0, 2, 22, 1) 50%);
  padding: 100px 12.361111111111% 40px 12.361111111111%;
  min-height: 110vh;
}

@media (max-width: 1366px) {
  #commands {
    padding: 90px 85px 10px 85px;
  }
}

@media (max-width: 768px) {
  #commands {
    padding: 30px 40px 10px 44px;
  }
}

@media (max-width: 610px) {
  #commands {
    padding: 0px 40px 10px 44px;
  }
}
</style>
