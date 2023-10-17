<script>
        import Step from "./Step.svelte";

let steps = [
    {
        name: "Smoljames Store",
        icon: "fa-solid fa-cart-shopping",
        description:
            "Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
    },
    {
        name: "Utlimate Todos",
        icon: "fa-solid fa-list-check",
        description:
            "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
    },
    {
        name: "Pokédex",
        icon: "fa-solid fa-diagram-project",
        description:
            "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
    },
];

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
];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">

       <div class="flex flex-col lg: justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
        <h2 class="font-semibold text-4x1 sm:text-5x1 md:text-6x1">
            Hi! I'm <span class="poppins text-violet-400">Daniel </span> Lins <br/>Full Stack
            <span class="poppings text-violet-400">Developer</span>
        </h2>
        <p class="text-base sm:text-lg md:text-xl">
            My <span class="text-violet-400">favorite tech</span> includes JavaScript (Next.JS or
            SvelteKit), React Native, Styled-Components, TailwindCss, Node.js + Express.js & PostgreSQL or Firebase
        </p>
        <a 
        class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins
        relative overflow-hidden px-6 py-3 groud rounded-full bg-white text-slate-950
        cursor-pointer" href="#">
    
        <div
        class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
    />
    <h4 class="relative z-9">Get in touch &rarr;</h4>

    </a>
       </div>
        <div class="relative shadow-2x1 grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />

        </div>

    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2x1">
                A few of my creative endeavors.

            </h6>
            <h3 class="font-semibold text-3x1 sm:text-4x1 md:text-5x1">
                Curios to <span class="poppins text-violet-400">see</span> my 
                work?
            </h3>
    
    
  </div>
    <a href="" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0
    -mt-10 hover:border-violet-700 duration-200">
    <i class="fa-regular fa-circle-play"></i>
    <p>Watch the video</p>

    </a>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
        <Step step={steps[0]}>
            <p>Smoljames Store is a merchandising store created with
            <strong class="text-violet-400">Next.js Commeerce.js Stripe & Node.js + Express.js !</strong> Commerce.js is a product CMS and Stripe is uesd all transaction </p>

        </Step>
        <Step step={steps[1]}>
        </Step>
        <Step step={steps[2]}>
        </Step>
    </div>

    </section>
</main>