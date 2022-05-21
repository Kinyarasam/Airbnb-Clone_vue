<template>
    <div class="flex justify-between shadow px-24 items-center">
        <div class="flex relative">
            <button type="button" name="button" class="absolute left-0 top-[30%] shadow-white shadow-xl bg-white flex justify-center items-center">
                <div class="hover:shadow-lg rounded-full shadow-white shadow bg-white border mr-4 flex justify-center h-8 w-8 items-center">
                    <span class="material-icons">chevron_left</span>
                </div>
            </button>
            <div v-for="(menu,i) in menubar" :key="i" >
                <button @click="selectedMenu = menu.key" :class="`${selectedMenu === menu.key ? 'border-b-2 border-black text-black' : 'text-[#777777] '}items-center py-3 mr-10 cursor-pointer hover:border-b-2 `">
                     <div class="flex justify-center items-center">
                        <img class="h-8 w-6" :src="`${menu.src}`" />
                    </div>
                    <div class="">
                        <span class="text-[11px] block font-semibold">{{ menu.name }}</span>
                    </div>
                </button>
            </div>
            <button type="button" name="button" class="absolute right-[-20px]  top-[30%]  flex justify-center items-center">
                <div class="hover:shadow-lg rounded-full border mr-4 flex justify-center shadow-white shadow-xl bg-white h-8 w-8 items-center">
                    <span class="material-icons">chevron_right</span>
                </div>
            </button>
        </div>
        <button type="button" name="button" class="flex justify-center items-center">
            <div class="rounded border text-sm flex py-3 px-2">
                <span class="material-icons text-[20px]">sort</span>
                <div class="px-2">Filters</div>
            </div>
        </button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            selectedMenu: 'Design',
            menubar: [
                { key: 'Design', src: "menuBar/Design.jpg", name: "Design" },
                { key: 'Arctic', src: "menuBar/Arctic.jpg", name: "Arctic"},
                { key: 'Shared_homes', src: "menuBar/shared_homes.jpg", name: "Shared Homes"},
                { key: 'OMG!', src: "menuBar/OMG!.jpg", name: "OMG!"},
                { key: 'National_parks', src: "menuBar/National_parks.jpg", name: "National parks"},
                { key: 'Bed', src: "menuBar/bed_and_breakfast.jpg", name: "Bed & breakfast"},
                { key: 'Caves', src: "menuBar/Caves.jpg", name: "Caves"},
                { key: 'Camping', src: "menuBar/Camping.jpg", name: "Camping" },
                { key: 'Tiny_homes', src: "menuBar/Tiny_homes.jpg", name: "Tiny homes"},
                { key: 'Earth_homes', src: "menuBar/Earth_homes.jpg", name: "Earth homes"}
            ]
        }
    }
}
</script>

<styles>

</styles>