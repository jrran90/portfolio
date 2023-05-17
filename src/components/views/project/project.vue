<template>
  <div class="grid">
    <div v-for="(list,index) in projects" :key="index" class="p-4">
      <div class="border-gray-200 rounded-lg overflow-hidden">
        <img class="h-80 w-full object-cover object-top bg-white dark:bg-gray-900" :src="list.img"
             alt="blog">
        <div class="p-6 h-full dark:bg-gray-900 bg-white opacity-75">
          <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 dark:text-gray-200 mb-1">
            {{ list.subTitle }}</h2>
          <h1 class="title-font text-lg font-medium text-gray-900 dark:text-gray-100 mb-3">
            {{ list.title }}</h1>
          <p class="leading-relaxed mb-3">{{ list.description }}</p>
          <div class="flex items-center flex-wrap ">
            <a class="text-blue-600 inline-flex items-center md:mb-2 lg:mb-0" target="_blank"
               :href="list.github">More
              <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"
                   fill="none" stroke-linecap="round" stroke-linejoin="round">
                <path d="M5 12h14"></path>
                <path d="M12 5l7 7-7 7"></path>
              </svg>
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Projects',
  data() {
    return {
      sample: false,
      projects: [
        {
          img: require('@/assets/img/projectsThumbnail/jacknpoy.png'),
          subTitle: 'VueJS, Laravel, MySQL',
          title: `Jack N' Poy`,
          description: `The Philippine version of rock-paper-scissors. It is an online platform where gamers may compete and win prizes by playing with other players.`,
          github: 'https://jacknpoy.com/'
        },
        {
          img: require('@/assets/img/projectsThumbnail/mlrewards.png'),
          subTitle: 'VueJS, Laravel, MongoDB, PayPal',
          title: 'ML Rewards',
          description: `It is an online platform that aims to bring forth games such as memory, analysis, and tactic genres in order to help the user enhance their intellect. It further connect components from Mobile Legend: Bang Bang, such as heroes, hero skills, roles, and so forth, to even provide players with a fully immersive experience while utilizing our platform.`,
          github: '#'
        },
        {
          img: require('@/assets/img/projectsThumbnail/nantiaja.png'),
          subTitle: 'VueJS, NodeJS, WooCommerce, Shopify, FinTech',
          title: 'NantiAja',
          description: `A financial service that divides payment into four installments on one of the supported merchants. Supported multiple e-commerce platforms i.e., Shopify, WooCommerce, Magento, PrestaShop and even custom one.`,
          github: '#'
        },
        {
          img: require('@/assets/img/projectsThumbnail/empatkali.png'),
          subTitle: 'VueJS, NodeJS, WooCommerce, FinTech',
          title: 'PT Empat Kali',
          description: `Modern payment solutions that allows you to pay 25% up-front, and settle the remaining 75% later with 0% interest. Supported multiple e-commerce platforms i.e., Shopify, WooCommerce, Magento, PrestaShop and even custom one.`,
          github: '#'
        },
        {
          img: require('@/assets/img/projectsThumbnail/vitacorpo.png'),
          subTitle: 'VueJS, NuxtJS',
          title: 'VitaCorpo - Web Application (Admin Dashboard)',
          description: `COVID-19 RESPONSE MANAGEMENT VitaCorpo simplifies and automates the hundreds of tasks involved in managing your daily COVID-19 response. I am also one of the front end dev working on the admin dashboard application.`,
          github: 'https://vitacorpo.com/'
        },
        {
          img: require('@/assets/img/projectsThumbnail/mojipass.png'),
          subTitle: 'VueJs, NuxtJs',
          title: 'Mojipass',
          description: `Mojipass is a frictionless platform for content providers and merchants to attract new customers through temporary, free, privacy-friendly, instant access to streaming services.`,
          github: 'https://mojipass.com/'

        },
        {
          img: require('@/assets/img/projectsThumbnail/dasboardmednefits.png'),
          subTitle: 'VueJS, AngularJS, Laravel',
          title: 'Mednefits App Migration',
          description: `App migration in their admin portal, the current app of mednefits been using angularJs from the start and company is growing fast and app is getting slower due to outdated version of angular, I'm part of the project whos working to migrate the app from angularJs to VueJs 2`,
          github: 'https://www.mednefits.com/'

        },
        {
          img: require('@/assets/img/projectsThumbnail/mednefits.png'),
          subTitle: 'VueJS, Laravel',
          title: 'Mednefits Analytics Dashboard',
          description: `Me and co-developer assigned to work on this project, We design and Develop this analytics dashboard from scratch using VueJs and chartJs or the charting, analytics for how many users are active ,in-active, their sales etc..`,
          github: '#'

        },
        {
          img: require('@/assets/img/projectsThumbnail/motormate.png'),
          subTitle: '',
          title: 'Motormate Group of Companies',
          description: `A motorcycle wholesaler, retailer and services such as, tune-up, change oil, etc. We created custom HRIS (Human Resource Information System) for 201, Payroll, etc.`,
          github: 'https://motormate-group.com'
        },
      ],
    }
  }
}
</script>
