<template>
    <div class="tablaled">
        
        <h1>Tabla led</h1>

        <table v-for="led in 27 " v-bind:class = "'table-screen px' + led" border="0" cellspacing="10">
            <tbody>
                <tr v-for="i in screen[0].height">
                    <td class='cpixel' v-for="j in screen[0].width" v-bind:data-i = i v-bind:data-j = j >
                        <!-- {{i}}-{{j}} -->
                    </td>
                </tr>

            </tbody>
        </table>

        <button v-on:click='renderAlphabet("A")'>Ejecutar</button>    
        <!-- <button v-on:click='go'>Ejecutar</button>     -->

    </div>
</template>

<script>

export default {
    data()
    {
        return{
            screen:[{
                width: 5,
                height: 7
            }],
            currentx:0
        }
    },
    methods:{
        renderAlphabet( caracter )
        {
            // A
            document.querySelector('.px1 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px1 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="5"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px1 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="5"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px1 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="5"][data-j="4"]').style.backgroundColor='black';
            
            document.querySelector('.px1 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="3"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="4"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="6"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px1 td[data-i="7"][data-j="5"]').style.backgroundColor='black';

            // B
            document.querySelector('.px2 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px2 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="4"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px2 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px2 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="4"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px2 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="3"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px2 td[data-i="6"][data-j="5"]').style.backgroundColor='black';

            // C
            document.querySelector('.px3 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="6"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px3 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px3 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px3 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px3 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px3 td[data-i="6"][data-j="5"]').style.backgroundColor='black';

            // D
            document.querySelector('.px4 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px4 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px4 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px4 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px4 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="3"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="4"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px4 td[data-i="6"][data-j="5"]').style.backgroundColor='black';

            // E
            document.querySelector('.px5 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px5 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="4"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px5 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px5 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="4"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px5 td[data-i="1"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px5 td[data-i="7"][data-j="5"]').style.backgroundColor='black';

            // E
            document.querySelector('.px6 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px6 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="4"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px6 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px6 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px6 td[data-i="4"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px6 td[data-i="1"][data-j="5"]').style.backgroundColor='black';

            // G
            document.querySelector('.px7 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="6"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px7 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px7 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px7 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="4"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px7 td[data-i="4"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px7 td[data-i="6"][data-j="5"]').style.backgroundColor='black';

            // H
            document.querySelector('.px8 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px8 td[data-i="4"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px8 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px8 td[data-i="4"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px8 td[data-i="1"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="3"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="4"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="6"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px8 td[data-i="7"][data-j="5"]').style.backgroundColor='black';

            // I

            document.querySelector('.px9 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px9 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="2"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="3"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="4"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="5"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="6"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="7"][data-j="3"]').style.backgroundColor='black';

            document.querySelector('.px9 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px9 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            // J

            document.querySelector('.px10 td[data-i="6"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px10 td[data-i="1"][data-j="2"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px10 td[data-i="1"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="7"][data-j="3"]').style.backgroundColor='black';

            document.querySelector('.px10 td[data-i="1"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="2"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="3"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="4"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="5"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px10 td[data-i="6"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px10 td[data-i="1"][data-j="5"]').style.backgroundColor='black';

            // k
            document.querySelector('.px11 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px11 td[data-i="4"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px11 td[data-i="3"][data-j="3"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="5"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px11 td[data-i="2"][data-j="4"]').style.backgroundColor='black';
            document.querySelector('.px11 td[data-i="6"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px11 td[data-i="7"][data-j="5"]').style.backgroundColor='black';

            // L
            document.querySelector('.px12 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px12 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px12 td[data-i="7"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px12 td[data-i="7"][data-j="3"]').style.backgroundColor='black';
            
            document.querySelector('.px12 td[data-i="7"][data-j="4"]').style.backgroundColor='black';

            // M
            document.querySelector('.px13 td[data-i="1"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="2"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="3"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="4"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="5"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="6"][data-j="1"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="7"][data-j="1"]').style.backgroundColor='black';

            document.querySelector('.px13 td[data-i="2"][data-j="2"]').style.backgroundColor='black';
            // document.querySelector('.px13 td[data-i="4"][data-j="2"]').style.backgroundColor='black';

            document.querySelector('.px13 td[data-i="3"][data-j="3"]').style.backgroundColor='black';

            document.querySelector('.px13 td[data-i="3"][data-j="4"]').style.backgroundColor='black';
            
            // document.querySelector('.px13 td[data-i="4"][data-j="4"]').style.backgroundColor='black';

            document.querySelector('.px13 td[data-i="1"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="2"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="3"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="4"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="5"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="6"][data-j="5"]').style.backgroundColor='black';
            document.querySelector('.px13 td[data-i="7"][data-j="5"]').style.backgroundColor='black';















            return false;

            if (this.currentx < this.screen[0].height ) 
            {
            
                this.currentx++;

                // console.log(this.currentx);

                this.clearScreen();

                var tdselect = document.querySelectorAll('.table-screen td[data-i="' + this.currentx + '"]');
                
                tdselect.forEach((td)=>{
                    
                    td.style.backgroundColor='red';
                    
                });

                window.setTimeout(this.renderAlphabet, 50);
                
            }
            else
            {

                this.currentx=0;

            }

        },
        clearScreen()
        {
            var pixels = document.querySelectorAll('.table-screen td');
                    
            pixels.forEach((pixel)=>{
                
                pixel.style.backgroundColor='rgb(197, 199, 199)';
                
            });
        },
        sleep(milliseconds) {
            const date = Date.now();
            let currentDate = null;
            do {
                currentDate = Date.now();
            } while (currentDate - date < milliseconds);
        }

    },
    created(){
    
        // this.renderAlphabet("A");
    
    }

}
</script>

<style>
    :root{
        --pixelheight: 2px ;
        --color: rgb(255, 255, 255);
        --spacecell: 0px;
    }
    .table-screen
    {
        border-spacing: var(--spacecell); 
        float: left;
        margin-right: 2px;
    } 
    .table-screen td{
        background:var(--color);
        height: var(--pixelheight);
        width: var(--pixelheight);
        border:none;
        padding: 0;
    }

</style>