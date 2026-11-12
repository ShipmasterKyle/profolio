<script lang="ts">
    import { Button, Hr, Popover, Card, Table, TableBody, TableBodyCell, TableBodyRow, TableHead, TableHeadCell } from "flowbite-svelte";
    import { PlaySolid, SunOutline } from "flowbite-svelte-icons"	
    import Icon from "@iconify/svelte";
    import { fade, blur } from "svelte/transition";

    import me from "#lib/assets/me.jpg"
    import goat from "#lib/assets/goat.png"
    import drg from "#lib/assets/drgametime3d.jpg"
    import ship from "#lib/assets/ship.png"
    import se from "#lib/assets/se.png"
    import gg from "#lib/assets/GGMB_Emblem.png"
    import chao from "#lib/assets/chao.jpg"
    import cbx from "#lib/assets/infinite.png"
    import ae from "#lib/assets/ace-engine.png"
    import sevo from "#lib/assets/sevo.png"
    import slw from "#lib/assets/slw.jpg"
    import pb from "#lib/assets/pixel-brwl.png"
    import pl from "#lib/assets/Pokemon Legends Logo.png"
    import gif from "#lib/assets/isle.gif"
    let page = $state(0);
</script>


<main class="grid h-screen grid-cols-1 md:grid-cols-2 font-sans">
    <section class="w-full h-full">
    {#if page == 0}
        <div style="background-image: url({gif});" class="size-full bg-cover flex-col items-baseline content-end p-6" transition:fade={{ duration: 300 }}>
            <h1 class="text-white mt-auto mb-0 text-4xl font-semibold tracking-tighter text-heading sm:text-4x1 md:text-5xl lg:text-6xl">Who is ShipmasterKyle</h1>
            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">Gabriel Thompson aka ShipmasterKyle, is a self-taught programmer currently leading development on the Cubix Infinite. He started programming back in 2019 and is currently studying Computer Science at Fort Valley State University to polish his skills. He's the founder and  <b>lead Software Engineer</b> at <b>Cubix Entertainment</b> where he contributes to building a new indie console. </p>
            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">Outside of work Gabriel is a musician where he both plays a variety of percussive and string instruments including piano, drums and guitar and creates original music as a producer. He's also a retired roblox band director (2021-2025), as well as the founder of the Roblox Music Assoication.</p>
            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">During his time at Fort Valley as an undergrad student, he'd like to improve as a Software Engineer with a formal education. He's most interested in Software Engineering and Game development although he's also spent researching Cybersecurity. Gabriel has spent several years working as a freelance programmer although his primary project at Cubix began in 2023.</p>
            <!-- <Hr class="mx-auto my-4 h-1 w-48 rounded-sm md:my-10" /> -->
            <h2 class="text-white mt-auto mb-0 text-4xl font-semibold tracking-tighter text-heading text-4x1">Technical Skills</h2>
            <Table>
                <TableHead class="bg-slate-800">
                    <TableHeadCell>Skill</TableHeadCell>
                    <TableHeadCell>Skill Level</TableHeadCell>
                    <TableHeadCell>Skill Since</TableHeadCell>
                </TableHead>
                <TableBody class="text-slate-300">
                    <TableBodyRow class="bg-slate-700">
                    <TableBodyCell>Lua Programming</TableBodyCell>
                    <TableBodyCell>Advanced</TableBodyCell>
                    <TableBodyCell>2019</TableBodyCell>
                    </TableBodyRow>
                    <TableBodyRow class="bg-slate-600">
                    <TableBodyCell>Web Development (Svelte)</TableBodyCell>
                    <TableBodyCell>Intermediate</TableBodyCell>
                    <TableBodyCell>2023</TableBodyCell>
                    </TableBodyRow>
                    <TableBodyRow class="bg-slate-700">
                    <TableBodyCell>C Programming</TableBodyCell>
                    <TableBodyCell>Intermediate</TableBodyCell>
                    <TableBodyCell>2024</TableBodyCell>
                    </TableBodyRow>
                    <TableBodyRow class="bg-slate-600">
                    <TableBodyCell>Python Programming</TableBodyCell>
                    <TableBodyCell>Developing</TableBodyCell>
                    <TableBodyCell>2021</TableBodyCell>
                    </TableBodyRow>
                    <TableBodyRow class="bg-slate-700">
                    <TableBodyCell>Javascript/Typescript Programming</TableBodyCell>
                    <TableBodyCell>Developing</TableBodyCell>
                    <TableBodyCell>2024</TableBodyCell>
                    </TableBodyRow>                    <TableBodyRow class="bg-slate-600">
                    <TableBodyCell>Unix System Management</TableBodyCell>
                    <TableBodyCell>Intermediate</TableBodyCell>
                    <TableBodyCell>2024</TableBodyCell>
                    </TableBodyRow>
                    <TableBodyRow class="bg-slate-700">
                    <TableBodyCell>Database Management</TableBodyCell>
                    <TableBodyCell>Intermediate</TableBodyCell>
                    <TableBodyCell>2024</TableBodyCell>
                    </TableBodyRow>

                </TableBody>
            </Table>
        </div>
    {:else if page == 1}
        <div class="size-full bg-baby flex flex-col items-baseline content-end" transition:fade={{ duration: 300 }}>
            <div class="w-full grid grid-cols-3 lg:grid-cols-4 gap-4 p-6 lg:py-2 mb-0">
                <Button id="popover-cb" class="col-span-3 lg:col-span-4">
                    <div class="size-full">
                        <img class="size-fill rounded-xl" src={cbx} alt="Sonic Earth">
                    </div>
                </Button>

                <Button id="popover-se">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={se} alt="Sonic Earth">
                        
                    </div>
                </Button>

                <Button id="popover-gg">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={gg} alt="Lumina University Band Hall">
                    </div>
                </Button>
                
                <Button id="popover-cg">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={chao} alt="Chao Engine">
                    </div>
                </Button>

                <Button id="popover-ae">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={ae} alt="Ace Engine">
                        
                    </div>
                </Button>

                <Button id="popover-ee">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={sevo} alt="Evo Engine">
                    </div>
                </Button>
                
                <Button id="popover-slw">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={slw} alt="Sonic Lost World">
                    </div>
                </Button>

                <Button id="popover-pb">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={pb} alt="Pixel Brawl">
                    </div>
                </Button>

                <Button id="popover-pl">
                    <div class="size-full aspect-square">
                        <img class="size-fill rounded-xl" src={pl} alt="Pokemon Legends">
                    </div>
                </Button>
            </div>
            <h1 class="w-full text-end text-white text-4xl font-medium tracking-tighter text-heading mt-auto mb-2 px-2 md:text-5xl lg:text-6xl">My Works</h1>
            <p class="text-base text-end lg:ml-auto font-normal text-body px-2 pb-2 md:text-xl text-white">I've been working as a Software Engineer since 2019. Here you can see just a few of my works!</p>
        </div>

        <Popover triggeredBy="#popover-se" class="w-64 bg-black text-sm font-light text-white border-0" transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Sonic Earth</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Roblox</p>
                </div>
                </div>
                <Button size="md" class="bg-ruby font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6" />Play</Button>
                <p class="text-sm">Sonic Fan Game with custom physics engine (Hedgeburst 2) that was developed from 2021-2024</p>
            </div>
        </Popover>

        <Popover triggeredBy="#popover-gg" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Lumina University Band Hall</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Roblox</p>
                </div>
                </div>
                <Button size="md" class="bg-ruby font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6" />Play</Button>
                <p class="text-sm">Award winning Roblox Band Hall fully equipt with animated instruments, custom admin commands and animations.</p>
            </div>
        </Popover>

        <Popover triggeredBy="#popover-cg" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Chao Engine</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Roblox Framework</p>
                </div>
                </div>
                <a href="https://codeberg.org/ShipmasterKyle/Chao-Engine" class="decoration-0">
                    <Button size="md" class="bg-ruby font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>View Code</Button>
                    <p class="text-sm">Roblox Framework for a Sonic Adventure 2 styled Chao Garden. </p>
                </a>
                
            </div>
        </Popover>

        <Popover triggeredBy="#popover-ae" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Ace Engine</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Scratch Framework</p>
                </div>
                </div>
                <a href="https://scratch.mit.edu/projects/568351098/" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>View Code</Button>
                    <p class="text-sm">Ace Attorney fan game framework inspired by pyWright and Attorney Online.</p>
                </a>
                
            </div>
        </Popover>

        
        <Popover triggeredBy="#popover-ee" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Sonic Evo Engine</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Scratch Framework</p>
                </div>
                </div>
                <a href="https://scratch.mit.edu/projects/568351098/" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>View Code</Button>
                    <p class="text-sm">2D Sonic Framework that attempts to bring piggeh's Modern Sonic Engine to Scratch 3</p>
                </a>
                
            </div>
        </Popover>

        <Popover triggeredBy="#popover-slw" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Sonic Lost World</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Scratch</p>
                </div>
                </div>
                <a href="https://scratch.mit.edu/projects/419395453/" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>Play</Button>
                    <p class="text-sm">2D "Demake" of Sonic Lost World</p>
                </a>
                
            </div>
        </Popover>

        <Popover triggeredBy="#popover-pb" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Pixel Battle</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Scratch</p>
                </div>
                </div>
                <a href="https://scratch.mit.edu/projects/937857872" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>Play</Button>
                    <p class="text-sm">Simple 2D Fighting game in collaboration with K1mar1s. My work is on all the menus and UI.</p>
                </a>
                
            </div>
        </Popover>
        
        <Popover triggeredBy="#popover-pl" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Pokemon Legends</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">Scratch</p>
                </div>
                </div>
                <a href="https://shipmasterkyle.github.io/Legends/" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>Visit Website</Button>
                    <p class="text-sm">Pokemon Fan Game inspired by Prodigy developed in 2023</p>
                </a>
                
            </div>
        </Popover>

        <Popover triggeredBy="#popover-cb" class="w-64 bg-black text-sm font-light text-white border-0"  transition={blur} transitionParams={{ duration: 250 }}>
            <div class="p-3">
                <div class="text-base leading-none font-semibold text-white">
                <p class="mb-2">Cubix Infinite</p>
                <div class="mb-3 text-sm font-normal inline">
                    <Icon icon="catppuccin:roblox" inline={true}/>
                    <p class="hover:underline">C</p>
                </div>
                </div>
                <a href="https://cubixdev.org" class="decoration-0">
                    <Button size="md" class="bg-gold font-sans"><PlaySolid class="m-0 shrink-0 h-6 w-6"/>Visit Website</Button>
                    <p class="text-sm">Independent Gaming Console with a fully custom OS built on Linux.</p>
                </a>
                
            </div>
        </Popover>
    {:else if page == 2}
        <div class="size-full bg-gray-950 p-6" transition:fade={{ duration: 300 }}>
            <h1 class="text-center text-white mb-0 text-4xl font-semibold tracking-tighter text-heading md:text-5xl lg:text-6xl">Academic Profile</h1>
            <div class="mb-1 text-base font-medium text-heading">
                <h2 class="text-3xl text-slate-200">Graduation Progress (49%)</h2>
            </div>
            <div class="w-full bg-zinc-500 rounded-full h-2.5">
                <div class="bg-blue-300 h-2.5 rounded-full" style="width: 49%"></div>
            </div>
            <br>
            <p class="text-slate-200 mt-2">As of November 2026, I have completed 49% of my degree's coursework reqork. Out of the classes completed only one has direct relationship to my major. At the expected pace I'm taking courses (with an average 17 credit hours) I should graduate Spring 2028.</p>

            <br><br>
            <h3 class="text-white mb-0 text-4xl font-semibold tracking-tighter text-heading">Courses Remaining</h3>
            <div class="grid grid-cols-2 lg:grid-cols-4 gap-4">
                <Card class="bg-green-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 1301</h5>
                    <p class="font-normal text-black">Principles of Programming I</p>
                </Card>
                <Card class="bg-amber-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 1302</h5>
                    <p class="font-normal text-black">Principles of Programming II</p>
                </Card>
                <Card class="bg-amber-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 2201</h5>
                    <p class="font-normal text-black">Digital Fundamentals</p>
                </Card>
                <Card class="bg-amber-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 1102</h5>
                    <p class="font-normal text-black">CSCI & CSIS: An Overview</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">MATH 1154</h5>
                    <p class="font-normal text-black">Calculus I</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">MATH 2253</h5>
                    <p class="font-normal text-black">Discrete Math</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">MATH 1401</h5>
                    <p class="font-normal text-black">Elementary Statistics</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 3150</h5>
                    <p class="font-normal text-black">Data Communication and Networks</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 3331</h5>
                    <p class="font-normal text-black">C Unix</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 3351</h5>
                    <p class="font-normal text-black">Comp Organization/Assembly Language</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 3410</h5>
                    <p class="font-normal text-black">Data Structures</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSIS 3743</h5>
                    <p class="font-normal text-black">Web Development</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 4320</h5>
                    <p class="font-normal text-black">Software Engineering</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 4340</h5>
                    <p class="font-normal text-black">Principles of Operating Systems</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSCI 4520</h5>
                    <p class="font-normal text-black">Analysis of Algorithms</p>
                </Card>
                <Card class="bg-red-400 border-0 p-4 sm:p-6 md:p-8">
                    <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-950">CSIS 4720</h5>
                    <p class="font-normal text-black">Database Systems</p>
                </Card>
            </div>
        </div>
    {:else if page == 3}
        <div class="size-full bg-gold p-6" transition:fade={{ duration: 300 }}>
            <h1 class="text-white mb-0 text-4xl font-semibold tracking-tighter text-heading sm:text-4x1 md:text-5xl lg:text-6xl">Freshman Reflection</h1>
            <p class="text-normal text-white">
                In my first real year of being a computer science program, I've learned a lot of interesting things about it. My primary reason for coming to a university to major in something I've already been doing professionally for years for to get a formal education to "fill in the gaps" left by my self teaching. I did admitably, find a lot of the entry level topics boring (you can only learn about what a CPU is so many times) but I did still get a lot out of it. I got to rediscover my love for Hexadecimal and reading an ASCII table. I think binary math was one of the most interesting topics I've learned this year. That said, the biggest challenege early on has been staying engaged. Theres so much overlap of things I already know, but staying engaged lets me enjoy the things I didn't know much about. As for my programming skills, I think I'm too far gone in my programming "style" for any outside source to drastically change how I write code. I don't believe my problem solving process has changed much this year either. The skills I need to develop are languages I've thrown to the wayside while focusing on the ones I love the most. I really want to develop my C programming skills since thats what I primarily use on a day to day basis. My social skills and ability to work with others also needs to improve but that will in time. 
            </p>
        </div>  
    {/if}
    </section>

    <section class="min-h-50dvh bg-black md:min-h-dvh flex flex-col justify-center items-center gap-4 md:gap-6 px-2">
    <div class="w-full flex justify-center items-center gap-4 md:gap-6 px-2">
        <div class="w-1/3 grid grid-cols-2 grid-rows-3 gap-2 lg:gap-0">
        <button class="cursor-pointer col-start-2 rounded-full ring-2 ring-gold" onclick={() => {page = 1}}>
            <img class="size-full aspect-square rounded-full object-cover" src={drg} alt="Drgametime3d">
        </button>

        <button class="cursor-pointer rounded-full ring-2 ring-gold" onclick={() => {page = 2}}>
            <img class="size-full aspect-square rounded-full object-cover" src={ship} alt="ShipmasterKyle">
        </button>

        <button class="cursor-pointer col-start-2 row-start-3 rounded-full ring-2 ring-gold" onclick={() => {page = 3}}>
            <img class="size-full aspect-square rounded-full object-cover" src={goat} alt="the_true_illusion">
        </button>
        </div>
        <button class="cursor-pointer w-2/3" onclick={() => {page = 0}}>
        <img class="size-full aspect-square rounded-full object-cover border-4 border-gold" src={me} alt="Gabriel Thompson">
        </button>
    </div>
    <h1 class="text-center text-gold mb-0 text-4xl font-bold tracking-tighter text-heading md:text-5xl lg:text-6xl"><SunOutline class="inline-flex self-center aspect-square mx-2" />ShipmasterKyle<SunOutline class="inline-flex self-center aspect-square mx-2" /></h1>
    <p class="mt-0 mb-8 text-base font-normal text-body md:text-xl text-white">Often Imitated, Never Duplicated.</p>
        
    </section>
</main>