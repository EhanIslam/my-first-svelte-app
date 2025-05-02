<script>

    let color2 = "white";
    const lightmode = () => {
            color2 = "white"
    }
    const darkmode = () => {
             color2 = "black"
    }
</script>
<div class="background">
    <div class="flex h-140 w-75 rounded-3xl p-3 flex-col overflow-hidden" style="background-color: {color2};">
        <div class="flex flex-row" >
            <div style="color: {color2 === "black" ? "white" : "black"}" class="fixed font-strong pl-1.5">5:48</div>
            <div class="fixed flex flex-row gap-1.25 pl-50 pt-1">
                <span style="background-color: {color2 === "black" ? "white" : "black"}" class="icon-[material-symbols--wifi] w-4.5 h-4.5"></span>
                <span style="background-color: {color2 === "black" ? "white" : "black"}" class="icon-[lets-icons--sound-max-fill] w-4.5 h-4.5"></span>
                <span style="background-color: {color2 === "black" ? "white" : "black"}" class="icon-[bx--battery] w-4.5 h-4.5"></span>
            </div>
    </div>
        <div class="flex pt-23 mr-auto ml-auto">
            <div class= "hover:bg-blue-100 hover:scale-112 ease-in-out transition duration-200 rounded-4xl h-7 w-19 bg-blue-200 flex flex-row justify-evenly pt-0.5">
                <button onclick={lightmode} aria-label="m" >
                    <span class="icon-[si--sun-fill] h-6 w-5" style="background-color: {color2}; opacity: {color2 === "white" ? 10 : 0.5}"></span>
                </button>
                <button onclick={darkmode} aria-label="m">
                    <span class="icon-[solar--moon-bold] h-5.75   w-5.5" style="background-color: {color2 === "black" ? "white" : "black"};opacity: {color2 === "black" ? 10 : 0.5}"></span>
                </button>
            </div>
        </div>
        <!-- This app was supposably to be a Calculator Project but I don't know much about Css Grids and that is why I failed for the Design so I turned it into something else -->
        <!-- <div class="h-full w-full grid grid-cols-5 grid-rows-4 pt-5v gap-0.5">
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc"></div>
                <div class="box-calc  col-span-2"></div>

        </div> -->
        <h1 class=" font-black text-3xl text-center pt-20 font-serif" style="color: {color2 === "black" ? "white" : "black"};">Wow! I build my First App in SvelteKit which also has Dark Mode Feature!</h1>
    </div>
</div>