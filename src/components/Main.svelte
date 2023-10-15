<script>
  let benefits = [
    {name: 'a cloud guru', description: "I'm well-versed with cloud technologies and how to maintain and deploy infrastructure in both public and private clouds. I have experience with AWS and GCP. I'm also familiar with Terraform and Pulumi."},
    {name: 'a backend maestro', description: "I'm experienced with building and maintaining backend services. I'm familiar with Python, Java, and Ruby. I'm also familiar with the Spring framework."},
    {name: 'a frontend fanatic', description: 'I love building beautful, functional, and accessible web applications. I am familiar with Javascript, Typescript, React, and Sveltekit.'},
    {name: 'an excellent teammate and communicator', description: "I'm a great teammate and communicator. I'm always willing to help and I'm always willing to learn. I'm also a great communicator and I'm always willing to share my ideas and thoughts as well as listen to others."}
  ]
</script>

<main class="flex flex-col flex-1 p-4">
  <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-violet-400">Kiel</span> Haymon <br/> Software
        <span class="poppins text-violet-400">Engineer</span>
      </h2>
      <p class="text-lg sm:text-xl md:text-xl">
        I'm a software engineer with a passion for building beautiful and functional cloud-native applications. My <span class="text-violet-400"> favorite tech</span>
          includes Python, Java, AWS, and GCP!
      </p>
      <a
      href="https://www.linkedin.com/in/kiel-haymon-02489b80/"
      target="_blank"
     class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer">
      <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
      />
      <h4 class="relative z-9">Get In Touch &rarr;</h4>
      </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img src={"images/profile_2.png"} alt="Profile Image" class="object-cover z-[2] max-h-[70vh]"/>
  </section>
  <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
          A bit <span class="poppins text-violet-400">about</span> me.
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am . . .
  </p>
    <p class="mx-auto poppinis font-semibold text-lg sm:text-xl md:text-2l"></p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
      <div class="flex gap-6 sm:gap-8">
        <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-600 font-semibold">
          0{index + 1}
        </p>
        <div class="flex flex-col gap-6 sm:gap-8">
          <h3 class="text-2xl sm:text-3xl md:text-4xl">
            {benefit.name}
          </h3>
          <p>{benefit.description}</p>
        </div>
      </div>
      {/each}
    </div>
  </section>
</main>