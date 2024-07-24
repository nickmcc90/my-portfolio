<script>
  export let y;

  let tabs = [
    {name: 'Projects', link: '#projects'},
    {name: 'About me', link: '#about'},
  ]
</script>

<header class={"sticky top-0 z-[10] duration-200 px-6 flex items-center justify-between border border-solid " + 
`${y > 0 ? ' py-4 bg-[#008080] border-[#3EB489]' : ' py-6 bg-transparent border-transparent'}`}>
  <h1 class='font-medium'>
    <b class='font-bold poppins'>Nicholas</b> McCarroll
  </h1>
  <div class='sm:flex items-center gap-4 hidden'>
    {#each tabs as tab, index}
      <a href={tab.link} class='duration-200 hover:text-[#000080]'>
        <p>{tab.name}</p>
      </a>
    {/each}
  </div>
  <a href='https://www.linkedin.com/in/nicholas-mccarroll/'
    target='_blank'
    class='pinkShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white
  text-slate-950'>
    <div class='absolute top-0 right-full w-full h-full bg-[#fe6453] opacity-20
    group-hover:translate-x-full z-0 duration-200 '></div>
    <h4 class='relative z-9'>Get in touch</h4>
  </a>
</header>