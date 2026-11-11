<script lang="ts">
    import { Button, Hr, Popover } from "flowbite-svelte";
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
    let page = $state(2);
</script>

<main class="grid h-screen grid-cols-1 md:grid-cols-2 font-sans">
    <section class="w-full h-full">
    {#if page == 0}
        <div class="size-full bg-gold p-6" transition:fade={{ duration: 300 }}>
            <h1 class="text-white mb-0 text-4xl font-semibold tracking-tighter text-heading sm:text-4x1 md:text-5xl lg:text-6xl">Who is ShipmasterKyle</h1>
            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">Gabriel Thompson aka ShipmasterKyle, is a self-taught programmer currently leading development on the Cubix Infinite. He started programming back in 2019 and is currently studying Computer Science at Fort Valley State University to polish his skills. He's the founder and  <b>lead Software Engineer</b> at <b>Cubix Entertainment</b> where he contributes to building a new indie console. </p>
            <br>
            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">Outside of work Gabriel is a musician where he both plays a variety of percussive and string instruments including piano, drums and guitar and creates original music as a producer. He's also a retired roblox band director (2021-2025), as well as the founder of the Roblox Music Assoication.</p>
            <Hr class="mx-auto my-4 h-1 w-48 rounded-sm md:my-10" />

            <p class="text-base font-normal text-body px-2 py-2 md:text-xl text-white">During his time at Fort Valley as an undergrad student, he'd like to improve as a Software Engineer with a formal education. He's most interested in Software Engineering and Game development although he's also spent researching Cybersecurity. Gabriel has spent several years working as a freelance programmer although his primary project at Cubix began in 2023.</p>
        </div>
    {:else if page == 1}
        <div class="size-full bg-baby flex flex-col items-baseline content-end" transition:fade={{ duration: 300 }}>
            <div class="w-full grid grid-cols-3 lg:grid-cols-4 gap-4 p-6 lg:py-2 mb-0">
                <Button id="popover-cb" class="col-span-3">
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
            <h1 class="text-center text-black mb-0 text-4xl font-semibold tracking-tighter text-heading md:text-5xl lg:text-6xl">Academic Profile</h1>
            <div class="mb-1 text-base font-medium text-heading">Large</div>
                <div class="w-full bg-zinc-500 rounded-full h-2.5">
                <div class="bg-blue-300 h-2.5 rounded-full" style="width: 45%"></div>
            </div>
        </div>
    {/if}
    </section>

    <section class="min-h-50dvh bg-black md:min-h-dvh flex flex-col justify-center items-center gap-4 md:gap-6 px-2">
    <div class="w-full flex justify-center items-center gap-4 md:gap-6 px-2">
        <div class="w-1/3 grid grid-cols-2 grid-rows-3 gap-2 lg:gap-0">
        <button class="col-start-2 rounded-full ring-2 ring-gold" onclick={() => {page = 1}}>
            <img class="size-full aspect-square rounded-full object-cover" src={drg} alt="Drgametime3d">
        </button>

        <button class="rounded-full ring-2 ring-gold" onclick={() => {page = 2}}>
            <img class="size-full aspect-square rounded-full object-cover" src={ship} alt="ShipmasterKyle">
        </button>

        <button class="col-start-2 row-start-3 rounded-full ring-2 ring-gold" onclick={() => {page = 3}}>
            <img class="size-full aspect-square rounded-full object-cover" src={goat} alt="the_true_illusion">
        </button>
        </div>
        <button class="w-2/3" onclick={() => {page = 0}}>
        <img class="size-full aspect-square rounded-full object-cover border-4 border-gold" src={me} alt="Gabriel Thompson">
        </button>
    </div>
    <h1 class="text-center text-gold mb-0 text-4xl font-bold tracking-tighter text-heading md:text-5xl lg:text-6xl"><SunOutline class="inline-flex self-center aspect-square mx-2" />ShipmasterKyle<SunOutline class="inline-flex self-center aspect-square mx-2" /></h1>
    <p class="mt-0 mb-8 text-base font-normal text-body md:text-xl text-white">Often Imitated, Never Duplicated.</p>
        
    </section>
</main>