<template>
    <div class="flex justify-between py-3 px-24 border-b text-sm font-medium">
        <div class="h-10 flex justify-center items-center">
            <img src="airbnb.png" alt="Logo" class="h-8">
        </div>
        <div class="h-6 pl-6 pr-2 py-6 flex justify-center items-center cursor-pointer border rounded-full shadow-md hover:shadow">
            <button class="border-r pr-3 text-black text-[13px] font-medium">Anywhere</button>
            <button class="border-r px-3 text-black text-[13px] font-medium">Any week</button>
            <button class="px-3 text-[#777777] font-light text-[13px]">Add guests</button>
            <button class="bg-rose-500 rounded-full h-8 w-8 flex justify-center items-center">
                <span class="material-icons text-white text-[17px] font-bold">search</span></button>
        </div>
        <div class="flex justify-center items-center cursor-pointer">
            <div class="p-3 text-black text-[13px] hover:bg-gray-100 rounded-full">Become a Host</div>
            <div class="p-3 rounded-full hover:bg-gray-100 flex justify-center items-center">
                <span class="material-icons">language</span>
            </div>
            <div class="relative hover:shadow-md rounded-full border flex justify-center items-center text-[#777777]">
                <span class="material-icons text-xl px-1 pl-2">menu</span>
                <span class="material-icons text-4xl px-1">account_circle</span>
                <div class="absolute top-0 right-0 bg-rose-500 h-3.5 w-3.5 border-2 border-white rounded-full"></div>
            </div>
        </div>
    </div>
</template>