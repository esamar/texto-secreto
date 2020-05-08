<template>
    <div class="tablaled">
        
        <h1>Tabla led</h1>

        <input type="text">

        <div class = "backscreen">

            <table v-for="led in messageLen" v-bind:class = "'table-screen px' + led" border="0" cellspacing="10">
                <tbody>
                    <tr v-for="i in screen[0].height">
                        <td class='cpixel' v-for="j in screen[0].width" v-bind:data-i = i v-bind:data-j = j >
                            <!-- {{i}}-{{j}} -->
                        </td>
                    </tr>

                </tbody>
            </table>

        </div>

        <button v-on:click='renderAlphabet("A")'>Ejecutar</button>    

    </div>
</template>

<script>

export default {
    data()
    {
        return{
            screen:[{
                width: 6,
                height: 7
            }],
            messageLen: 100,
            message:'ESTO ES UNA PRUEBA',
            currentx:0
        }
    },
    methods:{
        renderAlphabet( caracter )
        {
            for (let chr = 0; chr < this.message.length; chr++) 
            {

                console.log(this.message[chr].toUpperCase())
                var pxid = chr + 1;
                switch(this.message[chr].toUpperCase())
                {
                case 'A':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'B':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'C':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'D':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'E':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'E':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'G':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'H':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'I':

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'J':

                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'k':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'L':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'M':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';


                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'N':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                
                break; 
                case 'Ñ':
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

            break; 
            case 'O':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

            break; 
            case 'P':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

            break; 
            case 'Q':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

            break; 
            case 'R':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';


                break; 
                case 'S':
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'T':

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'W':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';


                
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'U':
                    document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';

                    // document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                    // document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                    
                    // document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                    document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                    document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 


                case 'X':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';


                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'Y':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';


                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                

                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case 'Z':
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="1"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="2"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="3"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="4"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="5"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';

                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                

                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="2"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="3"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="4"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="5"]').style.backgroundColor='rgb(129, 255, 91)';

                break; 
                case ',':

                document.querySelector('.px' + pxid + ' td[data-i="7"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                document.querySelector('.px' + pxid + ' td[data-i="6"][data-j="1"]').style.backgroundColor='rgb(129, 255, 91)';
                break;

                }
            }


            return false;

            if (this.currentx < this.screen[0].height ) 
            {
            
                this.currentx++;

                'console'.log(this.currentx);

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
    
    //  'this'.renderAlphabet("A");
    
    }

}
</script>

<style>
    :root{
        --pixelheight: 5px ;
        --color: transparent;
        --spacecell: 3px;
    }
    .table-screen
    {
        border-spacing: var(--spacecell); 
        float: left;
        margin-right: 0px;
        /* margin-bottom: 2px; */
    } 
    .table-screen td{
        background:var(--color);
        height: var(--pixelheight);
        width: var(--pixelheight);
        border:none;
        padding: 0;
    }

    .backscreen{
        background: rgb(0, 0, 0);
        padding: 5px;
        overflow: auto;
    }

</style>