<script>
    import Step from "./Step.svelte";
    
    let steps = [
        {name: 'Admin Dashbard', 
            icon: 'fa-solid fa-chart-line', 
            link: 'https://react-dashboard22.netlify.app/', 
            git: 'https://github.com/Ma7moudxG/react-admin2'},
        {name: 'Freescribe', 
            icon: 'fa-solid fa-language', 
            link: 'https://freescribe-react.netlify.app/', 
            git: 'https://github.com/Ma7moudxG/freescribe'},
        {name: 'Amino Gym', 
            icon: 'fa-solid fa-dumbbell', 
            link: 'https://amino-gym.netlify.app/', 
            git: 'https://github.com/Ma7moudxG/amino-gym'},
        {name: 'React NASA App', 
            icon: 'fa-solid fa-user-astronaut', 
            link: 'https://nasa-react-app-22.netlify.app/', 
            git: 'https://github.com/Ma7moudxG/react-nasa-app'},
        {name: 'Fruits Store', 
            icon: 'fa-solid fa-cart-shopping', 
            link: 'https://fruits-store-app.netlify.app/', 
            git: 'https://github.com/Ma7moudxG/fruits-shop'},
        {name: 'Rent A Bike', 
            icon: 'fa-solid fa-bicycle', 
            link: 'https://rent-a-bike-production.up.railway.app/', 
            git:'https://github.com/Ma7moudxG/rent--a-bike'},
        // {name: 'Pokedex', icon: 'fa-solid fa-diagram-project'},
    ]

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
        },
        {
            name: "a product design & UX finatic",
            description:
                "Carefully crafting and designing amazing user experiences allows me to express and experiment with every morsel of creativity I have. I love the challenge of learning new design concepts and enabling users with amazing online experiences.",
        },
        {
            name: "an excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
    ]

</script>

<main class="flex flex-col flex-1 p-4">
    <section id="interoPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <br /><span class="poppins text-amber-400">Mahmoud</span> Mahran<br /> Front End <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl ">
                My <span class="text-amber-400">favourite tech</span> includes JavaScript (NEXT.JS or Reat JS), TailwindCSS, Express & PostgreSQL or Firebase!
            </p>

            <a class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins 
            relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 
            cursor-pointer" 
            href="https://www.linkedin.com/in/ma7moudxG" target="_blank">
                <div class="absolute top-8 right-full w-full h-full bg-amber-400 opacity-20 group-hover:translate-x-full z-0 duartion-200" />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>

        <div class="reltive shadow-2xl grid place-items-center">
            <img src={"images/profile.png"} alt="Profile image" class="object-cover-z-[2] max-h-[70vh]"/>
        </div>
    </section>


    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl ">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-amber-400">see</span> my work?
            </h3>
        </div>
        
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>React Admin Full Dashboard, Made with
                    <strong class="text-violet-400">
                       React, Material UI, echarts, FullCalendar,Data Grid
                    </strong>
                    it consists of 4 different Charts, Profiles, Products, 3 different Data Table Pages, FAQ Page, Form Page, and Calendar Integration. 
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>Either you will record your voice, or upload an audio file to the website, you can Transcribe it, translate to any language you want, copy it to clipboard or download it in a file, Made with
                    <strong class="text-violet-400">
                        Reactjs, JavaScript, tailwindCss
                    </strong>
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>Amino Gym is a Planner for your gym workout, Made with
                    <strong class="text-violet-400">
                        Next.js, Vite, React.JS + TailwindCSS!
                    </strong>
                    From all workouts splits, pick your poison, targetted muscles, and your ultimate objctive, and the workout plan will be there for you. 
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>It is an app that shows a new wallpaper from NASA and their explorations, and you can know more info about this photo, Made with
                    <strong class="text-violet-400">
                        Reactjs, JavaScript, tailwindCSS
                    </strong>
                </p>
            </Step>
            <Step step={steps[4]}>
                <p>Fruits Store is a merchandising store created with
                    <strong class="text-violet-400">
                        Next.js, Stripe, Node.js + Express.js!
                    </strong>
                    Explore all kind of fresh fruits and finish your order in the smallest steps possible
                </p>
            </Step>
            <!-- <Step step={steps[5]}>
                <p>Rent A Bike is a full Stack
                    <strong class="text-violet-400">
                        Next.js, Node.js + MongoDB & TailwindCSS!
                    </strong>
                    Application that allows a user to login as a seller or a client, handle products and authentication and much more...
                </p>
            </Step> -->
            <!-- <Step step={steps[2]}>
                <p>The Pokédex is a <strong class="text-violet-400"
                    >SvelteKit & TailwindCSS</strong
                >
                web application, hosted on
                <strong class="text-violet-400">Netlify</strong>, that
                consumes and caches the
                <strong class="text-violet-400">Pokémon API</strong>
                to display all Pokémon information. Gotta catch them all!
                </p>
            </Step> -->
        </div>
    </section>

    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 
        before:h-1.5 before:bg-violet-700  after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl ">Want to know more?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-amber-400 ">about </span>me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-28 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                        0{index+1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8 ">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p class="">
                            {benefit.description}
                        </p>
                    </div>
                </div>
            {/each}
        </div>

        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
            The <span class="text-amber-400 poppins">Complete </span> Package
        </h5>
        <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="whitespace-nowrap bg-amber-500 text-white p-4 px-8">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 
                        pr-8 py-4 font-semibold text-sm whitespace-nowrap">
                            Dedication
                        </td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 
                        pr-8 py-4 font-semibold text-sm whitespace-nowrap">
                            Critical Thought
                        </td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 
                        pr-8 py-4 font-semibold text-sm whitespace-nowrap">
                            Interpersonal Skills
                        </td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 
                        pr-8 py-4 font-semibold text-sm whitespace-nowrap">
                            Programming Ability
                        </td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td ><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>
