<script setup>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Terminal from './components/Terminal.vue';
import Card from './components/Card.vue';
import Head2 from './components/Head2.vue';
</script>

<template>
  <body class="flex min-h-screen scroll-smooth flex-col bg-neutral-50 text-neutral-900 antialiased transition-colors duration-300 dark:bg-[#0a0a0b] dark:text-white">
    <Header></Header>
    <main class="flex-1">

    <!-- ===== Hero ===== -->
    <section class="mx-auto grid w-full max-w-7xl grid-cols-1 items-center gap-12 px-6 py-16 md:py-24 lg:grid-cols-2 lg:gap-16 lg:px-8">

      <!-- Left column -->
      <div class="max-w-xl">
        <span class="inline-flex items-center gap-2 rounded-full border border-accent-soft/20 bg-accent-soft/10 px-3 py-1 font-mono text-xs font-medium text-accent-soft">
          <span class="h-1.5 w-1.5 rounded-full bg-accent-soft"></span>
          Backend Developer
        </span>

        <h1 class="mt-6 text-5xl font-bold leading-[1.05] tracking-tight md:text-7xl">
          Hi, I'm
          <span class="mt-1 block font-['Dancing_Script'] text-6xl font-semibold text-accent-soft md:text-8xl">AmirHossein.</span>
        </h1>

        <p class="mt-6 max-w-lg text-base leading-relaxed text-neutral-500 dark:text-white/60">
          I am Amirhossein Mirjamali, a backend developer. I work with
          <span class="font-semibold text-accent-soft">Django</span> and focus primarily on designing and building robust
          <span class="font-semibold text-accent-soft">REST API</span> services.
        </p>

        <div class="mt-8 flex flex-wrap items-center gap-3">
          <a href="#skills" class="rounded-xl bg-linear-to-r from-accent-soft to-accent px-6 py-3 text-sm font-semibold text-neutral-900 transition hover:brightness-105">Explore Skills</a>
          <a href="#contact" class="rounded-xl border border-neutral-200 bg-white px-6 py-3 text-sm font-semibold text-neutral-900 transition-colors hover:bg-neutral-100 dark:border-white/10 dark:bg-white/5 dark:text-white dark:hover:bg-white/10">Get in Touch</a>
        </div>

        <!-- Stats -->
        <dl class="mt-10 grid max-w-md grid-cols-3 gap-6 border-t border-neutral-200 pt-6 dark:border-white/10">
          <div>
            <dt class="order-2 mt-1 text-xs text-neutral-500 dark:text-white/40">Year Experience</dt>
            <dd class="font-mono text-xl font-bold text-accent-soft">1+</dd>
          </div>
          <div>
            <dt class="mt-1 text-xs text-neutral-500 dark:text-white/40">Based In</dt>
            <dd class="font-mono text-xl font-bold text-accent-soft">Yazd, IR</dd>
          </div>
          <div>
            <dt class="mt-1 text-xs text-neutral-500 dark:text-white/40">Main Framework</dt>
            <dd class="font-mono text-xl font-bold text-emerald-500 dark:text-emerald-400">Django</dd>
          </div>
        </dl>
      </div>

      <!-- Right column: terminal -->
      <div class="w-full max-w-xl justify-self-center lg:justify-self-end">
        <Terminal title="amirhossein - profile">
          <div class="p-5 font-mono text-sm leading-7">
          <p><span class="text-emerald-400">$ whoami</span></p>
          <p class="text-white/80">Amirhossein Mirjamali</p>

          <p class="mt-4"><span class="text-emerald-400">$ cat profile.json</span></p>
    <pre class="mt-2 overflow-x-auto rounded-xl border border-white/10 bg-white/5 p-4 text-xs leading-6 text-white/70">{
    <span class="text-white/50">"role"</span>: <span class="text-accent-soft">"Backend Developer"</span>,
    <span class="text-white/50">"location"</span>: <span class="text-accent-soft">"Yazd, IR"</span>,
    <span class="text-white/50">"experience"</span>: <span class="text-accent-soft">"1+ year"</span>,
    <span class="text-white/50">"framework"</span>: <span class="text-accent-soft">"Django"</span>,
    <span class="text-white/50">"focus"</span>: <span class="text-accent-soft">"Micro Service & REST API"</span>
}</pre>

          <p class="mt-4"><span class="text-emerald-400">$ status</span></p>
          <p class="flex items-center gap-2 text-xs text-accent-soft">
            <span class="h-2 w-2 shrink-0 bg-accent-soft"></span>
            Ready for new challenges &amp; collaborations...
          </p>
        </div>
        </Terminal>
      </div>
    </section>

    <!-- ===== About ===== -->
    <section id="about" class="border-t border-neutral-200 py-20 transition-colors duration-300 dark:border-white/10">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="text-center">
          <p class="font-mono text-xs font-medium uppercase tracking-widest text-accent-soft">About Me</p>
          <Head2>Engineering robust solutions from the ground up</Head2>
        </div>

        <div class="mt-12 grid grid-cols-1 gap-6 md:grid-cols-3">
          <!-- Card 1 -->
          <Card>
            <span class="flex h-10 w-10 items-center justify-center rounded-lg bg-accent-soft/10 text-accent-soft">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-5 w-5">
                <path stroke-linecap="round" stroke-linejoin="round" d="M15 10.5a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z" />
                <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1 1 15 0Z" />
              </svg>
            </span>
            <h3 class="mt-5 text-lg font-semibold">Based in <span class="font-['Dancing_Script'] text-xl text-accent-soft">Yazd</span>, Iran</h3>
            <p class="mt-3 text-sm leading-relaxed text-neutral-500 dark:text-white/60">
              Living and working from the historic city of Yazd. Passionate about collaborating remotely with teams and companies globally and locally.
            </p>
          </Card>

          <!-- Card 2 -->
          <Card>
            <span class="flex h-10 w-10 items-center justify-center rounded-lg bg-accent-soft/10 text-accent-soft">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-5 w-5">
                <path stroke-linecap="round" stroke-linejoin="round" d="M17.25 6.75 22.5 12l-5.25 5.25m-10.5 0L1.5 12l5.25-5.25m7.5-3-4.5 16.5" />
              </svg>
            </span>
            <h3 class="mt-5 text-lg font-semibold">
              <span class="font-['Dancing_Script'] text-xl text-accent-soft">Python</span> &amp;
              <span class="font-['Dancing_Script'] text-xl text-accent-soft">Django</span>
            </h3>
            <p class="mt-3 text-sm leading-relaxed text-neutral-500 dark:text-white/60">
              Deep mastery of Python including advanced Object-Oriented Programming (OOP), asynchronous programming (Asyncio), and expert-level usage of the Django framework.
            </p>
          </Card>

          <!-- Card 3 -->
          <Card>
            <span class="flex h-10 w-10 items-center justify-center rounded-lg bg-emerald-400/10 text-emerald-500 dark:text-emerald-400">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-5 w-5">
                <path stroke-linecap="round" stroke-linejoin="round" d="M12 21a9.004 9.004 0 0 0 8.716-6.747M12 21a9.004 9.004 0 0 1-8.716-6.747M12 21c2.485 0 4.5-4.03 4.5-9S14.485 3 12 3m0 18c-2.485 0-4.5-4.03-4.5-9S9.515 3 12 3m0 0a8.997 8.997 0 0 1 7.843 4.582M12 3a8.997 8.997 0 0 0-7.843 4.582m15.686 0A11.953 11.953 0 0 1 12 10.5c-2.998 0-5.74-1.1-7.843-2.918m15.686 0A8.959 8.959 0 0 1 21 12c0 .778-.099 1.533-.284 2.253m0 0A17.919 17.919 0 0 1 12 16.5c-3.162 0-6.133-.815-8.716-2.247m0 0A9.015 9.015 0 0 1 3 12c0-1.605.42-3.113 1.157-4.418" />
              </svg>
            </span>
            <h3 class="mt-5 text-lg font-semibold"><span class="font-['Dancing_Script'] text-xl text-emerald-500 dark:text-emerald-400">Full-Stack</span> Capability</h3>
            <p class="mt-3 text-sm leading-relaxed text-neutral-500 dark:text-white/60">
              While focused on backend and REST API design, I am also well-versed in frontend technologies including HTML, CSS, JavaScript, and Vue.js to build complete solutions.
            </p>
          </Card>
        </div>
      </div>
    </section>

    <!-- ===== Skills ===== -->
    <section id="skills" class="border-t border-neutral-200 py-20 transition-colors duration-300 dark:border-white/10">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="text-center">
          <p class="font-mono text-xs font-medium uppercase tracking-widest text-accent-soft">Expertise &amp; Stack</p>
          <Head2>Technologies I work with daily</Head2>
        </div>

        <div class="mt-12 grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-4">

          <!-- 01 Backend & Python -->
          <Card>
            <div class="flex items-center gap-3">
              <span class="flex h-8 w-8 items-center justify-center rounded-lg bg-accent-soft/10 font-mono text-xs font-semibold text-accent-soft">01</span>
              <h3 class="text-sm font-semibold">Backend &amp; Python</h3>
            </div>
            <ul class="mt-5 space-y-2.5 text-xs">
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Python (OOP, Async)</span>
                <span class="font-mono text-[10px] text-accent-soft">Expert</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Django Framework</span>
                <span class="font-mono text-[10px] text-accent-soft">Advanced</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">API Design (REST)</span>
                <span class="font-mono text-[10px] text-accent-soft">Expert</span>
              </li>
            </ul>
          </Card>

          <!-- 02 Data & Caching -->
          <Card>
            <div class="flex items-center gap-3">
              <span class="flex h-8 w-8 items-center justify-center rounded-lg bg-accent-soft/10 font-mono text-xs font-semibold text-accent-soft">02</span>
              <h3 class="text-sm font-semibold">Data &amp; Caching</h3>
            </div>
            <ul class="mt-5 space-y-2.5 text-xs">
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">PostgreSQL</span>
                <span class="font-mono text-[10px] text-accent-soft">Advanced</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">SQL &amp; ORM</span>
                <span class="font-mono text-[10px] text-accent-soft">Advanced</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Redis (Caching/Queues)</span>
                <span class="font-mono text-[10px] text-accent-soft">Skilled</span>
              </li>
            </ul>
          </Card>

          <!-- 03 DevOps & Infra -->
          <Card>
            <div class="flex items-center gap-3">
              <span class="flex h-8 w-8 items-center justify-center rounded-lg bg-emerald-400/10 font-mono text-xs font-semibold text-emerald-500 dark:text-emerald-400">03</span>
              <h3 class="text-sm font-semibold">DevOps &amp; Infra</h3>
            </div>
            <ul class="mt-5 space-y-2.5 text-xs">
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Docker</span>
                <span class="font-mono text-[10px] text-emerald-500 dark:text-emerald-400">Skilled</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Linux OS &amp; Shell</span>
                <span class="font-mono text-[10px] text-emerald-500 dark:text-emerald-400">Advanced</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Nginx Web Server</span>
                <span class="font-mono text-[10px] text-emerald-500 dark:text-emerald-400">Skilled</span>
              </li>
            </ul>
          </Card>

          <!-- 04 Frontend Stack -->
          <Card>
            <div class="flex items-center gap-3">
              <span class="flex h-8 w-8 items-center justify-center rounded-lg bg-accent-soft/10 font-mono text-xs font-semibold text-accent-soft">04</span>
              <h3 class="text-sm font-semibold">Frontend Stack</h3>
            </div>
            <ul class="mt-5 space-y-2.5 text-xs">
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">HTML5 &amp; CSS3</span>
                <span class="font-mono text-[10px] text-amber-500 dark:text-amber-300">Proficient</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">JavaScript (ES6+)</span>
                <span class="font-mono text-[10px] text-amber-500 dark:text-amber-300">Proficient</span>
              </li>
              <li class="flex items-center justify-between rounded-lg border border-neutral-200 bg-neutral-100 px-3 py-3 dark:border-white/10 dark:bg-white/5">
                <span class="text-neutral-700 dark:text-white/80">Vue.js</span>
                <span class="font-mono text-[10px] text-amber-500 dark:text-amber-300">Proficient</span>
              </li>
            </ul>
          </Card>

        </div>
      </div>
    </section>

    <!-- ===== Projects ===== -->
    <section id="projects" class="border-t border-neutral-200 py-20 transition-colors duration-300 dark:border-white/10">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="text-center">
          <p class="font-mono text-xs font-medium uppercase tracking-widest text-accent-soft">Featured Work</p>
          <Head2>Recent Projects</Head2>
        </div>

        <div class="mx-auto mt-12 max-w-2xl">
          <Card >
            <div class="flex items-start justify-between">
              <span class="rounded-full border border-accent-soft/20 bg-accent-soft/10 px-3 py-1 font-mono text-[11px] text-accent-soft">Backend API</span>
              <a href="#" aria-label="AmirMovie on GitHub" class="text-neutral-400 transition-colors hover:text-neutral-900 dark:text-white/40 dark:hover:text-white">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="h-5 w-5">
                  <path d="M12 .5C5.65.5.5 5.65.5 12c0 5.08 3.29 9.39 7.86 10.91.58.1.79-.25.79-.56v-2c-3.2.7-3.87-1.37-3.87-1.37-.52-1.33-1.28-1.69-1.28-1.69-1.04-.71.08-.7.08-.7 1.15.08 1.76 1.18 1.76 1.18 1.03 1.76 2.69 1.25 3.35.96.1-.74.4-1.25.73-1.54-2.55-.29-5.24-1.28-5.24-5.69 0-1.26.45-2.28 1.18-3.09-.12-.29-.51-1.46.11-3.05 0 0 .97-.31 3.17 1.18a11 11 0 0 1 5.77 0c2.2-1.49 3.17-1.18 3.17-1.18.62 1.59.23 2.76.11 3.05.74.81 1.18 1.83 1.18 3.09 0 4.42-2.69 5.39-5.25 5.68.41.36.78 1.06.78 2.14v3.17c0 .31.21.67.8.56A11.5 11.5 0 0 0 23.5 12C23.5 5.65 18.35.5 12 .5Z" />
                </svg>
              </a>
            </div>

            <h3 class="mt-5 text-xl font-semibold">AmirMovie</h3>
            <p class="mt-3 text-sm leading-relaxed text-neutral-500 dark:text-white/60">
              A movie reservation API system built with Django and Django REST Framework. Features robust database architecture, integration with PostgreSQL, Elasticsearch for search functionality, and unit testing with Pytest.
            </p>

            <div class="mt-6 flex flex-wrap gap-2 border-t border-neutral-200 pt-5 dark:border-white/10">
              <span class="rounded-md border border-neutral-200 bg-neutral-100 px-2.5 py-1 font-mono text-[11px] text-accent-soft dark:border-white/10 dark:bg-white/5">Django</span>
              <span class="rounded-md border border-neutral-200 bg-neutral-100 px-2.5 py-1 font-mono text-[11px] text-accent-soft dark:border-white/10 dark:bg-white/5">PostgreSQL</span>
              <span class="rounded-md border border-neutral-200 bg-neutral-100 px-2.5 py-1 font-mono text-[11px] text-emerald-600 dark:border-white/10 dark:bg-white/5 dark:text-emerald-400">Elasticsearch</span>
              <span class="rounded-md border border-neutral-200 bg-neutral-100 px-2.5 py-1 font-mono text-[11px] text-accent-soft dark:border-white/10 dark:bg-white/5">Pytest</span>
            </div>
          </Card>
        </div>
      </div>
    </section>

    <!-- ===== Contact ===== -->
    <section id="contact" class="border-t border-neutral-200 py-20 transition-colors duration-300 dark:border-white/10 dark:bg-white/[0.02]">
      <div class="mx-auto max-w-3xl px-6 text-center lg:px-8">
        <p class="font-mono text-xs font-medium uppercase tracking-widest text-accent-soft">Get In Touch</p>
        <Head2>Let's build something exceptional together</Head2>
        <p class="mx-auto mt-5 max-w-xl text-base leading-relaxed text-neutral-500 dark:text-white/60">
          Whether you have a project in mind, want to discuss backend architecture, or just want to connect, my inbox is always open.
        </p>

        <div class="mt-8 flex flex-wrap items-center justify-center gap-3">
          <a href="mailto:thea9n@gmail.com"
            class="inline-flex items-center gap-2 rounded-xl bg-linear-to-r from-accent-soft to-accent px-6 py-3 text-sm font-semibold text-neutral-900 transition hover:brightness-105">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="h-4 w-4">
              <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 0 1-2.25 2.25h-15a2.25 2.25 0 0 1-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0 0 19.5 4.5h-15a2.25 2.25 0 0 0-2.25 2.25m19.5 0v.243a2.25 2.25 0 0 1-1.07 1.916l-7.5 4.615a2.25 2.25 0 0 1-2.36 0L3.32 8.91a2.25 2.25 0 0 1-1.07-1.916V6.75" />
            </svg>
            Email Me
          </a>
          <a href="https://github.com/amirhosin100/" class="inline-flex items-center gap-2 rounded-xl border border-neutral-200 bg-white px-6 py-3 text-sm font-semibold text-neutral-900 transition-colors hover:bg-neutral-100 dark:border-white/10 dark:bg-white/5 dark:text-white dark:hover:bg-white/10">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="h-4 w-4">
              <path d="M12 .5C5.65.5.5 5.65.5 12c0 5.08 3.29 9.39 7.86 10.91.58.1.79-.25.79-.56v-2c-3.2.7-3.87-1.37-3.87-1.37-.52-1.33-1.28-1.69-1.28-1.69-1.04-.71.08-.7.08-.7 1.15.08 1.76 1.18 1.76 1.18 1.03 1.76 2.69 1.25 3.35.96.1-.74.4-1.25.73-1.54-2.55-.29-5.24-1.28-5.24-5.69 0-1.26.45-2.28 1.18-3.09-.12-.29-.51-1.46.11-3.05 0 0 .97-.31 3.17 1.18a11 11 0 0 1 5.77 0c2.2-1.49 3.17-1.18 3.17-1.18.62 1.59.23 2.76.11 3.05.74.81 1.18 1.83 1.18 3.09 0 4.42-2.69 5.39-5.25 5.68.41.36.78 1.06.78 2.14v3.17c0 .31.21.67.8.56A11.5 11.5 0 0 0 23.5 12C23.5 5.65 18.35.5 12 .5Z" />
            </svg>
            GitHub
          </a>
          <a href="https://www.linkedin.com/in/amirhossein404/" class="inline-flex items-center gap-2 rounded-xl border border-neutral-200 bg-white px-6 py-3 text-sm font-semibold text-neutral-900 transition-colors hover:bg-neutral-100 dark:border-white/10 dark:bg-white/5 dark:text-white dark:hover:bg-white/10">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" class="h-4 w-4">
              <path d="M20.45 20.45h-3.56v-5.57c0-1.33-.03-3.04-1.85-3.04-1.86 0-2.14 1.45-2.14 2.94v5.67H9.34V9h3.41v1.56h.05c.48-.9 1.64-1.85 3.37-1.85 3.6 0 4.27 2.37 4.27 5.46v6.28ZM5.34 7.43a2.06 2.06 0 1 1 0-4.12 2.06 2.06 0 0 1 0 4.12ZM7.12 20.45H3.56V9h3.56v11.45ZM22.22 0H1.77C.79 0 0 .77 0 1.73v20.54C0 23.23.79 24 1.77 24h20.45c.98 0 1.78-.77 1.78-1.73V1.73C24 .77 23.2 0 22.22 0Z" />
            </svg>
            LinkedIn
          </a>
        </div>
      </div>
    </section>

  </main>
    <Footer></Footer>
  </body>
  
</template>
