<div class="drawer">
    <input id="my-drawer-3" type="checkbox" class="drawer-toggle" /> 
    <div class="drawer-content flex flex-col">
      <!-- Navbar -->
      <div class="w-full navbar bg-info ">
        <div class="flex-none lg:hidden justify-center"> <!-- Added justify-center here -->
          <label for="my-drawer-3" aria-label="open sidebar" class="btn btn-square btn-ghost">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-6 h-6 stroke-current"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path></svg>
          </label>
        </div> 
       
        <div class=" justify-end md:block flex-1 px-2 mx-2 ">
        <img src="logo.webp" alt="Logo" class="h-14 w-auto" />
    </div>
        <div class="flex-none hidden md:block">
          <ul class="menu menu-horizontal items-center text-white text-lg">
            
            <!-- Navbar menu content here -->
            <li><a>Dashboard</a></li>
            <li><a>Parts</a></li>
            <li><a>Estimation</a></li>
            <li><a>Setting</a></li>
            <li><a>Help</a></li>
            

            <li><a><img src="user.png" alt="Account Icon" class="h-10 w-10"></a></li> <!-- Account image icon -->
            
          </ul>
        </div>
      </div>

  
    </div> 
    <div class="drawer-side">
      <label for="my-drawer-3" aria-label="close sidebar" class="drawer-overlay"></label> 
      <ul class="menu p-4 w-80 min-h-full bg-base-300 text-lg">
        <!-- Sidebar content here -->
        <li><a><img src="user.png" alt="Account Icon" class="h-8 w-8"></a></li> <!-- Account image icon -->
        <li><a>Dashboard</a></li>
        <li><a>Parts</a></li>
        <li><a>Estimation</a></li>
        <li><a>Setting</a></li>
        <li><a>Help</a></li>
       
      </ul>
    </div>
</div>


