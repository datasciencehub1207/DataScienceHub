<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Data Science Hub - IIT MADRAS BS Resources</title>
  <link rel="stylesheet" href="/assets/index.css">
</head>
<body>
  <div id="root">
    <!-- Main App Structure from App.tsx and Layout.tsx -->
    <div class="min-h-screen flex flex-col">
      <!-- Header Component -->
      <header class="bg-white shadow-sm sticky top-0 z-30">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
          <div class="flex justify-between items-center py-3 md:space-x-10">
            <!-- Logo Section -->
            <div class="flex justify-start lg:w-0 lg:flex-1">
              <a class="flex items-center" href="/">
                <img class="h-10 w-auto" src="/src/assets/logo.svg" alt="Data Science Hub Logo">
                <div class="ml-3 flex flex-col">
                  <span class="text-[#800000] font-sans font-bold text-lg leading-tight">Data Science</span>
                  <span class="text-[#14397d] text-xs font-medium leading-tight">Hub</span>
                </div>
              </a>
            </div>

            <!-- Mobile Menu Button -->
            <div class="-mr-2 -my-2 md:hidden">
              <button type="button" class="inline-flex items-center justify-center rounded-md border border-neutral-200 p-2 text-neutral-400 hover:bg-neutral-100 hover:text-neutral-500">
                <span class="sr-only">Open menu</span>
                <svg class="h-5 w-5" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M3 5H17M3 10H17M3 15H17" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                </svg>
              </button>
            </div>

            <!-- Desktop Navigation Links -->
            <nav class="hidden md:flex space-x-6">
              <a class="text-[#800000] font-medium" href="/">Home</a>
              <a class="text-[#14397d] hover:text-[#800000] font-medium" href="/notes">Notes</a>
              <a class="text-[#14397d] hover:text-[#800000] font-medium" href="/pyqs">PYQs</a>
              <a class="text-[#14397d] hover:text-[#800000] font-medium" href="/code-notes">Code Notes</a>
              <a class="text-[#14397d] hover:text-[#800000] font-medium" href="/gpa-calculator">GPA Calculator</a>
            </nav>

            <!-- Desktop Search Bar -->
            <div class="hidden md:flex items-center justify-end md:flex-1 lg:w-0">
              <div class="relative w-64">
                <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                  <svg class="w-4 h-4 text-neutral-500" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M17.5 17.5L12.5 12.5M14.1667 8.33333C14.1667 11.555 11.555 14.1667 8.33333 14.1667C5.11167 14.1667 2.5 11.555 2.5 8.33333C2.5 5.11167 5.11167 2.5 8.33333 2.5C11.555 2.5 14.1667 5.11167 14.1667 8.33333Z" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                  </svg>
                </div>
                <input type="text" class="pl-10 pr-4 py-2 w-full border border-neutral-300 rounded-md focus:outline-none focus:ring-2 focus:ring-[#800000]" placeholder="Search resources...">
              </div>
            </div>
          </div>
        </div>
      </header>

      <!-- Main Content -->
      <main class="flex-1">
        <!-- Home Page Content (when on homepage) -->
        <div>
          <!-- Hero Section -->
          <div class="bg-[#800000] relative overflow-hidden">
            <div class="absolute inset-y-0 right-0 hidden w-1/2 overflow-hidden lg:block">
              <img class="h-full w-full object-cover opacity-20" src="https://images.unsplash.com/photo-1544383835-bda2bc66a55d?ixlib=rb-1.2.1&auto=format&fit=crop&w=1121&q=80" alt="Data Science Hub Campus">
            </div>
            <div class="container mx-auto px-4 sm:px-6 lg:px-8 relative">
              <div class="py-16 md:py-20 lg:py-24 max-w-3xl">
                <h1 class="text-3xl md:text-4xl lg:text-5xl font-sans font-bold text-white leading-tight">
                  Academic Resources for IIT Madras BS Students
                </h1>
                <p class="mt-4 text-white text-lg md:text-xl opacity-90">
                  Access comprehensive notes, previous year questions, code snippets, and a GPA calculator
                  to help you excel in your studies.
                </p>
                <div class="mt-8 flex flex-wrap gap-4">
                  <a href="/notes">
                    <button class="bg-white text-[#800000] hover:bg-neutral-100 px-5 py-6 font-medium">
                      Browse Resources
                    </button>
                  </a>
                  <a href="/gpa-calculator">
                    <button class="bg-[#14397d] hover:bg-[#0c2654] px-5 py-6 font-medium text-white">
                      Calculate GPA
                    </button>
                  </a>
                </div>
              </div>
            </div>
          </div>

          <!-- Resources Section -->
          <div class="py-12 bg-white">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
              <h2 class="text-2xl md:text-3xl font-sans font-bold text-center text-neutral-800 mb-12">
                Explore Resources
              </h2>
              <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 md:gap-8">
                <!-- Resource Card -->
                <a href="/notes" class="flex flex-col items-center p-6 bg-neutral-50 border border-neutral-200 rounded-lg hover:shadow-md transition-shadow duration-200">
                  <div class="w-16 h-16 flex items-center justify-center bg-opacity-10 rounded-full mb-4 bg-[#a02020]">
                    <svg class="h-8 w-8 text-[#800000]" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M7 18H17V16H7V18ZM7 14H17V12H7V14ZM7 10H17V8H7V10ZM5 22C4.45 22 3.979 21.804 3.587 21.412C3.195 21.02 2.999 20.549 3 20V4C3 3.45 3.196 2.979 3.588 2.587C3.98 2.195 4.451 1.999 5 2H19C19.55 2 20.021 2.196 20.413 2.588C20.805 2.98 21.001 3.451 21 4V20C21 20.55 20.804 21.021 20.412 21.413C20.02 21.805 19.549 22.001 19 22H5Z" fill="currentColor"/>
                    </svg>
                  </div>
                  <h3 class="text-lg font-sans font-medium text-neutral-800 mb-2">Course Notes</h3>
                  <p class="text-sm text-neutral-600 text-center">Comprehensive study materials for all courses</p>
                </a>
                
                <!-- More Resource Cards would be here -->
              </div>
            </div>
          </div>

          <!-- Featured Notes Section -->
          <section id="featured-notes" class="py-12 bg-neutral-50">
            <div class="container mx-auto px-4 sm:px-6 lg:px-8">
              <div class="mb-10">
                <h2 class="text-2xl md:text-3xl font-sans font-bold text-neutral-800 mb-4">
                  Course Notes
                </h2>
                <p class="text-lg text-neutral-600">
                  Comprehensive study materials organized by foundation, diploma, and degree levels.
                </p>
              </div>
              
              <!-- Notes Tabs -->
              <div>
                <div class="border-b border-gray-200 w-full mb-8">
                  <nav class="-mb-px flex space-x-8">
                    <a href="#" class="py-4 px-1 border-[#800000] text-[#800000] border-b-2 font-medium">
                      Foundation Level
                    </a>
                    <a href="#" class="py-4 px-1 border-transparent border-b-2 text-neutral-500 hover:text-neutral-700 font-medium">
                      Diploma Level
                    </a>
                    <a href="#" class="py-4 px-1 border-transparent border-b-2 text-neutral-500 hover:text-neutral-700 font-medium">
                      Degree Level
                    </a>
                  </nav>
                </div>
                
                <!-- Notes Cards Grid -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                  <!-- Notes Card -->
                  <div class="bg-white rounded-lg shadow-sm overflow-hidden">
                    <div class="bg-neutral-50 border-b border-neutral-200 p-5">
                      <h3 class="font-sans font-medium text-lg text-neutral-800">Linear Algebra</h3>
                    </div>
                    <div class="p-5">
                      <ul class="space-y-3">
                        <li class="flex items-start">
                          <svg class="h-5 w-5 text-[#800000] mt-0.5 mr-2" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path>
                          </svg>
                          <a href="/notes/1" class="text-[#14397d] hover:text-[#800000] hover:underline">
                            Linear Algebra Basics
                          </a>
                        </li>
                        <!-- More notes would be listed here -->
                      </ul>
                      <div class="mt-5">
                        <a href="/notes?course=Linear%20Algebra" class="text-sm text-[#800000] hover:text-[#690000] font-medium flex items-center">
                          View all resources
                          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" viewBox="0 0 20 20" fill="currentColor">
                            <path fill-rule="evenodd" d="M10.293 5.293a1 1 0 011.414 0l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414-1.414L12.586 11H5a1 1 0 110-2h7.586l-2.293-2.293a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                          </svg>
                        </a>
                      </div>
                    </div>
                  </div>
                  <!-- More note cards would be here -->
                </div>
              </div>
            </div>
          </section>
        </div>
      </main>

      <!-- Footer -->
      <footer class="bg-[#0c2654] text-white">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8 py-12">
          <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div>
              <div class="flex items-center mb-4">
                <img class="h-8 w-auto" src="/src/assets/logo.svg" alt="Data Science Hub Logo">
                <div class="ml-3">
                  <p class="font-sans font-bold text-lg leading-tight">Data Science</p>
                  <p class="text-xs font-medium leading-tight text-white text-opacity-80">
                    Hub
                  </p>
                </div>
              </div>
              <p class="text-sm text-white text-opacity-80 mb-4">
                Academic resources for students enrolled in the IIT Madras BS in Data Science program.
              </p>
              <div class="flex space-x-4">
                <a href="#" class="text-white hover:text-[#f3b617]" aria-label="Twitter">
                  <svg class="h-5 w-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M22 4.01C21 4.5 20.02 4.69 19 4.82C20.07 4.19 20.85 3.13 21.23 1.88C20.24 2.52 19.15 2.97 18 3.2C17.06 2.12 15.84 1.5 14.5 1.5C11.95 1.5 9.77 3.51 9.77 6.05C9.77 6.45 9.83 6.84 9.91 7.22C6.7 7.09 3.83 5.38 1.92 2.9C1.58 3.56 1.4 4.19 1.4 4.94C1.4 6.31 2.17 7.48 3.32 8.2C2.53 8.13 1.8 7.92 1.17 7.6C1.17 7.62 1.17 7.63 1.17 7.65C1.17 9.82 2.91 11.64 5.15 12.08C4.69 12.18 4.27 12.25 3.81 12.25C3.47 12.25 3.14 12.22 2.83 12.16C3.49 13.97 5.31 15.26 7.47 15.29C5.79 16.45 3.68 17.12 1.4 17.12C1.09 17.12 0.78 17.1 0.48 17.06C2.67 18.29 5.28 19 8.07 19C14.47 19 17.93 13.58 17.93 8.79C17.93 8.6 17.93 8.42 17.92 8.24C18.9 7.49 19.79 6.59 20.46 5.52L22 4.01Z" fill="currentColor"/>
                  </svg>
                </a>
                <a href="#" class="text-white hover:text-[#f3b617]" aria-label="Instagram">
                  <svg class="h-5 w-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z" fill="currentColor"/>
                  </svg>
                </a>
                <a href="#" class="text-white hover:text-[#f3b617]" aria-label="LinkedIn">
                  <svg class="h-5 w-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M19 3C19.5304 3 20.0391 3.21071 20.4142 3.58579C20.7893 3.96086 21 4.46957 21 5V19C21 19.5304 20.7893 20.0391 20.4142 20.4142C20.0391 20.7893 19.5304 21 19 21H5C4.46957 21 3.96086 20.7893 3.58579 20.4142C3.21071 20.0391 3 19.5304 3 19V5C3 4.46957 3.21071 3.96086 3.58579 3.58579C3.96086 3.21071 4.46957 3 5 3H19ZM18.5 18.5V13.2C18.5 12.3354 18.1565 11.5062 17.5452 10.8948C16.9338 10.2835 16.1046 9.94 15.24 9.94C14.39 9.94 13.4 10.46 12.92 11.24V10.13H10.13V18.5H12.92V13.57C12.92 12.8 13.54 12.17 14.31 12.17C14.6813 12.17 15.0374 12.3175 15.2999 12.5801C15.5625 12.8426 15.71 13.1987 15.71 13.57V18.5H18.5ZM6.88 8.56C7.32556 8.56 7.75288 8.383 8.06794 8.06794C8.383 7.75288 8.56 7.32556 8.56 6.88C8.56 5.95 7.81 5.19 6.88 5.19C6.43178 5.19 6.00193 5.36805 5.68499 5.68499C5.36805 6.00193 5.19 6.43178 5.19 6.88C5.19 7.81 5.95 8.56 6.88 8.56ZM8.27 18.5V10.13H5.5V18.5H8.27Z" fill="currentColor"/>
                  </svg>
                </a>
                <a href="#" class="text-white hover:text-[#f3b617]" aria-label="Facebook">
                  <svg class="h-5 w-5" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M22 12C22 6.48 17.52 2 12 2C6.48 2 2 6.48 2 12C2 16.84 5.44 20.87 10 21.8V15H8V12H10V9.5C10 7.57 11.57 6 13.5 6H16V9H14C13.45 9 13 9.45 13 10V12H16V15H13V21.95C18.05 21.45 22 17.19 22 12Z" fill="currentColor"/>
                  </svg>
                </a>
              </div>
            </div>
            <div>
              <h3 class="text-lg font-sans font-medium mb-4">Quick Links</h3>
              <ul class="space-y-2">
                <li>
                  <a href="/" class="text-white text-opacity-80 hover:text-white text-sm">Home</a>
                </li>
                <li>
                  <a href="/notes" class="text-white text-opacity-80 hover:text-white text-sm">Course Notes</a>
                </li>
                <li>
                  <a href="/pyqs" class="text-white text-opacity-80 hover:text-white text-sm">
                    Previous Year Questions
                  </a>
                </li>
                <li>
                  <a href="/code-notes" class="text-white text-opacity-80 hover:text-white text-sm">Code Notes</a>
                </li>
                <li>
                  <a href="/gpa-calculator" class="text-white text-opacity-80 hover:text-white text-sm">GPA Calculator</a>
                </li>
                <li>
                  <a href="#" class="text-white text-opacity-80 hover:text-white text-sm">
                    About Us
                  </a>
                </li>
                <li>
                  <a href="#" class="text-white text-opacity-80 hover:text-white text-sm">
                    Contact
                  </a>
                </li>
              </ul>
            </div>
            <div>
              <h3 class="text-lg font-sans font-medium mb-4">Contact</h3>
              <ul class="space-y-2">
                <li class="flex items-start">
                  <svg class="h-5 w-5 mr-2 text-white text-opacity-80" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M20 4H4C2.9 4 2.01 4.9 2.01 6L2 18C2 19.1 2.9 20 4 20H20C21.1 20 22 19.1 22 18V6C22 4.9 21.1 4 20 4ZM20 8L12 13L4 8V6L12 11L20 6V8Z" fill="currentColor"/>
                  </svg>
                  <span class="text-white text-opacity-80 text-sm">dshubhelp@gmail.com</span>
                </li>
              </ul>
              <div class="mt-6">
                <h3 class="text-lg font-sans font-medium mb-4">Subscribe to Updates</h3>
                <form class="flex">
                  <input type="email" placeholder="Your email" class="rounded-r-none text-neutral-800 px-4 py-2 w-full">
                  <button class="bg-[#f3b617] hover:bg-[#d99f0d] rounded-l-none px-4 py-2">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
                      <path fill-rule="evenodd" d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z" clip-rule="evenodd"></path>
                    </svg>
                  </button>
                </form>
              </div>
            </div>
          </div>
          <div class="mt-8 pt-8 border-t border-white border-opacity-20 text-center">
            <p class="text-sm text-white text-opacity-60">
              &copy; 2025 Data Science Hub Resources. All rights reserved.
            </p>
          </div>
        </div>
      </footer>
    </div>
  </div>

  <!-- Scripts -->
  <script type="module" src="/src/main.tsx"></script>
</body>
</html>
