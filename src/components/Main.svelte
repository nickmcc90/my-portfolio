<script>
  import Step from './Step.svelte'

  let steps = [
    {name: "Music API", icon: 'fa-solid fa-music', href: 'https://music-api-600.netlify.app'},
    {name: "Crazy Miser", icon: 'fa-solid fa-money-bill-trend-up', href: 'https://crazymiser.com'}
  ]

  let benefits = [
    {name: 'An engineer', desc: `I obtained a bachelors degree from 
    Purdue Univerity's mechanical engineering program. I began my career 
    by becoming a R&D project engineer working with water flow 
    right outside of graduating college. I worked for a year and one month before
    making the pivot into software development, which has been a passion of mine for
    a while! My decision is fueled by an immense
    curiosity and drive to understand how the online experience works and what the future
    of how we interact tech looks like.`, icon: 'fa-solid fa-pencil'},
    {name: 'Easy to get along with', desc: `My heart is huge! I find great joy in chatting
    and bonding with people wherever I go. I love to brighten people's days and bring
    out the most at-ease version of themselves. I love banter, and finding the magic
    in ordinary situations.`, icon: `fa-regular fa-face-smile-wink`},
    {name: 'A self taught developer', desc: `My passion for web development 
    started with a club at Purdue called Software Saturdays that I attended my 
    spring semester senior year. I had found their newsletter in my school email 
    inbox and thought it would be an important skill to learn, so I gave going
    to the meetings a shot. It was something different than my Mech E course work. I
    ended up finishing the final project (a pokedex app with React), getting their
    intermediate ReactJS certification, and fostering a new hobby for web creation. I've
    been learning more ever since and just started documenting my journey January 2024 on github.`,
    icon: 'fa-solid fa-file-code'}
  ]
</script>

<main class='flex flex-col flex-1 p-4'>
  <section id='introPage' class='grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14'>
    <div class='flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg-gap-10'>
      <h2 class='font-semibold text-4xl sm:text-5xl md:text-6xl'>
        Hi! I'm <span class='poppins text-[#fe6453]'>Nicholas</span> McCarroll <br/>
        Full Stack <span class='poppins text-[#fe6453]'>Developer</span>
      </h2>
      <p class='text-base sm:text-lg md:text-xl'>
        My favorite tech includes Javascript (NEXT.JS or SvelteKit), TailwindCSS,
        Node.js + Express.js & Firebase/Firestore!
      </p>
      <a href='https://www.linkedin.com/in/nicholas-mccarroll/' class='pinkShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins
      relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950'
      target="_blank">
        <div class='absolute top-0 right-full w-full h-full bg-[#008080] opacity-20
        group-hover:translate-x-full z-0 duration-200 '></div>
        <div class='flex items-center'>
          <h4 class='relative z-9'>Get in touch &rarr;</h4>
          <i class="fa-brands fa-linkedin ml-4 text-2xl"></i>
        </div>
      </a>
    </div>
    <div class='relative shadow-2xl grid place-items-center'>
      <img class='object-cover z-[0] max-h-[70vh]' src={'images/nickpicture.jpeg'} alt='Profile image' />
    </div>
  </section>

  <section id="projects" class='py-20 lg:py-32 flex flex-col gap-24'>
    <div class='flex flex-col gap-2 text-center'>
      <h6 class='text-large sm:text-xl md:text-2xl'>
        Here's what I've been working on:
      </h6>
    </div>
    <div class='grid grid-cols lg:grid-cols-2 gap-12 lg:gap-10'>
      <Step step={steps[0]}>
        <p>Music API is an api key store where you can purhcase a key that 
          gives you songs based on the vibe you want, either on a prepaid plan or a 
          subscription plan with metered usage. Created with <strong class='text-[#4ee2ac]'>Node.js + Express.js
          + React + TailwindCSS! Stripe</strong> is used for customer transactions and 
          <strong class='text-[#4ee2ac]'>Firebase</strong> is used
          to store customer and purchase data. API is deployed on an <strong class='text-[#4ee2ac]'>AWS EC2</strong> instance.
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>Crazy miser is the go-to website for reliable stock
          pick advice. It has topical articles, a weekly newsletter,
          and a forum to talk about certain topics.
          Made with basic <strong class='text-[#4ee2ac]'>HTML, CSS</strong> and
          <strong class='text-[#4ee2ac]'>Javascript. Firebase</strong>
          provides authentication and database storage and <strong class='text-[#4ee2ac]'>Paypal</strong> handles customer subscription transactions.
        </p>
      </Step>
    </div>
  </section>

  <section class='py-20 lg:py-32 flex flex-col gap-24 w-[700px] items-center mx-auto'>
    <div class='flex flex-col gap-2 text-center'>
      <h6 class='text-xl sm:text-2xl md:text-3xl'>
        Want to see more? Check the following projects out on my github pinned!
        <a href='https://github.com/nickmcc90'
        target='_blank'>
        <i class="fa-brands fa-github"></i>
      </a>
      </h6>
      <div>I've also worked with...</div>
      <ul>
        <li>
          <strong class='text-[#4ee2ac]'>Next.js and GCP </strong>- Made an e-commerce app that sells music I made. Video previews are loaded from GCP storage.
          <span class='underline'>Repo titled: music-store</span>
        </li>
        <li>
          <strong class='text-[#4ee2ac]'>React Native </strong>- Made a mobile app that you can search up movie reviews on.
          <span class='underline'>Repo titled: movie-info-app</span>
        </li>
        <li>
          <strong class='text-[#4ee2ac]'>Flask</strong>- Developing a Flask API that will send emails to customers from the Next.js e-commerce app.
          <span class='underline'>Repo titled: music-store-backend-python</span>
        </li>
      </ul>
    </div>
  </section>

  <section id='about' class='py-22 pt-10 lg:pt-16 lg-py-36 flex flex-col
  gap-16 sm:gap-20 md:gap-24 relative'>
    <div class='flex flex-col gap-2 text-center relative pt-8'>
      <h3 class='font-semibold text-3xl sm:text-4xl md:text-5xl'>A bit about me:</h3>
    </div>
    <p class='mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl'>I am...</p>
    <div class='flex flex-col gap-20 w-full mx-auto max-w-[800px]'>
      {#each benefits as benefit}
        <div class='flex gap-6 sm:gap-8'>
          <div class='text-4xl sm:text-5xl md:text-6xl w-[60px]'>
            <i class={`${benefit.icon}` + ' w-full  text-black flex justify-center'}></i>
          </div>
          <div class='flex flex-col gap-6 sm:gap-8 w-[708px]'>
            <h3 class='text-2xl sm:text-3xl md:text-5xl'>
              {benefit.name}
            </h3>
            <p class='text-justify'>{benefit.desc}</p>
          </div>
        </div>
      {/each}
    </div>
  </section>
</main>
