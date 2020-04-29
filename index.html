<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" type="text/css" href="./styles/styles.css" />
</head>
</head>

<body>

    <canvas id="canvas">
    </canvas>
    <div class="slidecontainer">
        <div class="hide_elements">
            <label for="pict_size_incr">Pict size</label>
            <input id="pict_size_incr" type="number" min="0" max="20" step="0.1" value="0.5" />
            <label for="pict_space_incr">Pict espaciado incrementador</label>
            <input id="pict_space_incr" type="number" min="0" max="100" step="0.1" value="0.1" />
        </div>


        <input type="file" id="file-input" accept="audio/*,video/*,image/*" />
        <h3 id="name"></h3>
        <audio id="audio" controls></audio>
    </div>
</body>
<script>

    let analyser;
    let dataArray;
    window.onload = function () {

        //WEB AUDIO ELEMENTS
        const file = document.getElementById("file-input");
        const h3 = document.getElementById('name')
        const audio = document.getElementById("audio");
        //END WEB AUDIO ELEMENTS

        let idol1 = new Image();
        let idol2 = new Image();
        let idol3 = new Image();
        let idol4 = new Image();
        let idol5 = new Image();
        let idol6 = new Image();
        let idol7 = new Image();
        let idol8 = new Image();
        let idol9 = new Image();
        let idol10 = new Image();
        let idol11 = new Image();
        let idol12 = new Image();
        let idol13 = new Image();
        let idol14 = new Image();
        let idol15 = new Image();
        let idol16 = new Image();
        let idol17 = new Image();
        let idol18 = new Image();
        let back1 = new Image();
        function init() {
            idol1.src = 'img/img2.gif';
            idol2.src = 'img/img1.jpg';
            idol3.src = 'img/img3.jpg';
            idol4.src = 'img/img4.jpg';
            idol5.src = 'img/img5.jpg';
            idol6.src = 'img/img6.jpg';
            idol7.src = 'img/img7.jpg';
            idol8.src = 'img/img8.jpg';
            idol9.src = 'img/img9.jpg';
            idol10.src = 'img/img10.jpg';
            idol11.src = 'img/img11.jpg';
            idol12.src = 'img/img12.png';
            idol13.src = 'img/img13.jpg';
            idol14.src = 'img/img14.jpg';
            idol15.src = 'img/img15.jpg';
            idol16.src = 'img/img16.jpg';
            idol17.src = 'img/img17.jpg';
            idol18.src = 'img/img18.jpg';
            back1.src = 'img/back1.jpg';

            window.requestAnimationFrame(draw);
        }

        //BACKGROUND IMAGE SIZE
        let back_pict_size = []
        back1.onload = function() {
            back_pict_size.push(back1.width);
            back_pict_size.push(back1.height);
        }

        //number of images
        let idols_picts = [idol1, idol2, idol3, idol4, idol5, idol6, idol7, idol8, idol9, idol10, idol11, idol12, idol13, idol14, idol15, idol16, idol17, idol18];
        //let idols_picts = [idol1];
        let num_of_picts = idols_picts.length;

        //array define time to spaw picts
        let time_to_spaw_pict = [];
        for (let x = 0; x < num_of_picts; x++) {
            let div_canvas = (((window.innerWidth + 100) / 2) / num_of_picts);
            if (x === 0) {
                time_to_spaw_pict.push(0);
            }
            else {
                time_to_spaw_pict.push(time_to_spaw_pict[x - 1] + div_canvas);
            }

        }
        console.log(time_to_spaw_pict);

        //array estado activacion label
        let array_status_layer = 0;

        //incrementador posicion horizontal - rotar
        let inc_horizontal_pos = 0.1;
        let array_increment_horizontal = [];
        for (let x = 0; x < num_of_picts; x++) {
            array_increment_horizontal.push(0);
        }
        //incrementador tamaño imagenes 
        let inc3 = parseFloat(document.getElementById("pict_size_incr").value);
        console.log("size pict incr: ", inc3);
        let array_size_pict = [];
        let size_pict_ini_val = 0;
        for (let x = 0; x < num_of_picts; x++) {
            array_size_pict.push(size_pict_ini_val);
        }

        //incrementador espaciado desde el centro - loop
        let inc2 = 1;
        let array_increment_pos = [];
        for (let x = 0; x < num_of_picts; x++) {
            array_increment_pos.push(0);
        }
        //incrementar EQUALIZER music
        let array_eq_incrementer = [];
        for (let x = 0; x < num_of_picts; x++) {
            array_eq_incrementer.push(0);
        } 

        //incrementar de espacio separacion exponencial
        //inc_space_tmp = parseFloat(document.getElementById("pict_space_incr").value);
        inc_space_tmp = 0.0;
        let array_inc_space_tmp = [];
        for (let x = 0; x < num_of_picts; x++) {
            array_inc_space_tmp.push(0);
        }

        //BACKGROUND SATURATION PING PONG HUE
        let back_hue_value = 0;
        let back_hue_incr = 0.1;
        let back_hue_max_value = 357;
        let back_hue_min_value = 1;

        file.onchange = function() {

            const files = this.files; // FileList containing File objects selected by the user (DOM File API)
            console.log('FILES[0]: ', files[0])
            audio.src = URL.createObjectURL(files[0]); // Creates a DOMString containing the specified File object

            const name = files[0].name
            h3.innerText = `${name}` // Sets <h3> to the name of the file

            ///////// <CANVAS> INITIALIZATION //////////
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
            const ctx = canvas.getContext("2d");
            ///////////////////////////////////////////


            const context = new AudioContext(); // (Interface) Audio-processing graph
            let src = context.createMediaElementSource(audio); // Give the audio context an audio source,
            // to which can then be played and manipulated
            analyser = context.createAnalyser(); // Create an analyser for the audio context

            src.connect(analyser); // Connects the audio context source to the analyser
            analyser.connect(context.destination); // End destination of an audio graph in a given context
            // Sends sound to the speakers or headphones


            /////////////// ANALYSER FFTSIZE ////////////////////////
            // analyser.fftSize = 32;
            // analyser.fftSize = 64;
            // analyser.fftSize = 128;
            // analyser.fftSize = 256;
            //analyser.fftSize = 512;
            // analyser.fftSize = 1024;
            // analyser.fftSize = 2048;
             analyser.fftSize = 4096;
            // analyser.fftSize = 8192;
            //analyser.fftSize = 16384;
            // analyser.fftSize = 32768;

            // (FFT) is an algorithm that samples a signal over a period of time
            // and divides it into its frequency components (single sinusoidal oscillations).
            // It separates the mixed signals and shows what frequency is a violent vibration.

            // (FFTSize) represents the window size in samples that is used when performing a FFT

            // Lower the size, the less bars (but wider in size)
            ///////////////////////////////////////////////////////////


            const bufferLength = analyser.frequencyBinCount; // (read-only property)
            // Unsigned integer, half of fftSize (so in this case, bufferLength = 8192)
            // Equates to number of data values you have to play with for the visualization

            // The FFT size defines the number of bins used for dividing the window into equal strips, or bins.
            // Hence, a bin is a spectrum sample, and defines the frequency resolution of the window.

            dataArray = new Uint8Array(bufferLength); // Converts to 8-bit unsigned integer array
            // At this point dataArray is an array with length of bufferLength but no values
            console.log('DATA-ARRAY: ', dataArray) // Check out this array of frequency values!

            const WIDTH = canvas.width;
            const HEIGHT = canvas.height;
            console.log('WIDTH: ', WIDTH, 'HEIGHT: ', HEIGHT)

            const barWidth = (WIDTH / bufferLength) * 13;
            console.log('BARWIDTH: ', barWidth)

            console.log('TOTAL WIDTH: ', (117*10)+(118*barWidth)) // (total space between bars)+(total width of all bars)

            let barHeight;
            let x = 0;


            audio.play();
            };
        

        function draw() {
            inc3 = parseFloat(document.getElementById("pict_size_incr").value);
            //inc_space_tmp = parseFloat(document.getElementById("pict_space_incr").value);
            var canvas = document.getElementById('canvas');
            var ctx = canvas.getContext('2d');
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;

            ///ctx.globalCompositeOperation = 'destination-over';
            ctx.clearRect(0, 0, window.innerWidth, window.innerHeight); // limpiar canvas

            // ctx.fillStyle = 'rgba(0,0,0,0.4)';
            // ctx.strokeStyle = 'rgba(0,153,255,0.4)';
            //ctx.save();
            ctx.translate(window.innerWidth / 2, innerHeight / 2);

            var maxCircle = 20;
            var radius = 300;
            var size = 100;

            //web audio 
            // var freqByteData = new Uint8Array(analyser.frequencyBinCount);
            // analyser.getByteFrequencyData(freqByteData);
            let freq_div = 200;
            
            if (analyser != null || analyser != undefined){
                analyser.getByteFrequencyData(dataArray); // Copies the frequency data into dataArray

                //let sum = dataArray.reduce((previous, current) => current += previous);
                //let sum = dataArray[0] + dataArray[dataArray.length - 1] + dataArray[(dataArray.length/2) - 1];
                //let avg = sum / 3;
                //console.log(avg/freq_div);
                //console.log(dataArray[2]/freq_div);
            }
            //BACKGROUND RENDER ==========
            
            var time = new Date();
            //ctx.rotate(20 * Math.PI / 180);

            ctx.rotate( ((2*Math.PI)/60)*time.getSeconds() + ((2*Math.PI)/60000)*time.getMilliseconds() );
            ctx.drawImage(back1, -back_pict_size[0]/2, -back_pict_size[1]/2);
            //rigth side
            ctx.drawImage(back1, back_pict_size[0]/2, -back_pict_size[1]/2);
            //left side
            ctx.drawImage(back1, -(back_pict_size[0]/2 + back_pict_size[0]), -back_pict_size[1]/2);
            //upper part
            ctx.drawImage(back1, -(back_pict_size[0]/2), -(back_pict_size[1]/2 + back_pict_size[1]));
            //bottom part
            ctx.drawImage(back1, -(back_pict_size[0]/2), back_pict_size[1]/2);
            //esquina upper-left
            ctx.drawImage(back1, -(back_pict_size[0]/2 + back_pict_size[0]), -(back_pict_size[1]/2 + back_pict_size[1]));
            //esquina upper-right
            ctx.drawImage(back1, (back_pict_size[0]/2), -(back_pict_size[1]/2 + back_pict_size[1]));
            //esquina bottom left
            ctx.drawImage(back1, -(back_pict_size[0]/2 + back_pict_size[0]), (back_pict_size[1]/2));
            //esquina bttom right
            ctx.drawImage(back1, (back_pict_size[0]/2), (back_pict_size[1]/2));
            // ctx.globalCompositeOperation = "saturation";
            // ctx.fillStyle = "hsl(126, 52%, 50%)";  // saturation at 100%
            // ctx.fillRect(-back_pict_size[0]/2, -back_pict_size[1]/2,back_pict_size[0], back_pict_size[1]);  // apply the comp filter
            // ctx.globalCompositeOperation = "source-over";  // restore default comp

            //LAYER 1
            for (let n = 0; n < num_of_picts; n++) {
                if ((array_increment_pos[0] >= time_to_spaw_pict[n]) && array_status_layer === 0) {
                    if (n === (num_of_picts - 1)) {
                        array_status_layer = 1;
                        console.log("reached last layer, interval between layers set!");
                    }
                    updateIdolsCircles(n);


                }
                else if (array_status_layer === 1) {
                    //console.log("entro al else");
                    updateIdolsCircles(n);
                }

            }

            function updateIdolsCircles(n) {
                //web audio frequencys


                array_increment_pos[n] = array_increment_pos[n] + inc2 + array_inc_space_tmp[n];
                if (dataArray != null || dataArray != undefined){
                    //let sum = dataArray.reduce((previous, current) => current += previous);
                    //let avg = sum / dataArray.length;
                    let eq_db = (dataArray[2]/freq_div);
                    //let eq_db = (avg/freq_div);
                    if (array_eq_incrementer[n] > eq_db) {
                        array_size_pict[n] = array_size_pict[n] + eq_db*1.7;
                        array_eq_incrementer[n] = eq_db;
                    }
                    else {
                        array_size_pict[n] = array_size_pict[n] - eq_db;
                        array_eq_incrementer[n] = eq_db;
                    }
                    //let sum = dataArray[0] + dataArray[dataArray.length - 1] + dataArray[(dataArray.length/2) - 1];
                    //let avg = sum / 3;
                    //array_size_pict[n] = array_size_pict[n] + (dataArray[2]/freq_div * 0.5) - (dataArray[(dataArray.length/2) - 1]/freq_div * 2);
                }
                else {
                    array_size_pict[n] = array_size_pict[n] + inc3;
                }
                
                array_inc_space_tmp[n] = array_inc_space_tmp[n] + inc_space_tmp;
                array_increment_horizontal[n] = array_increment_horizontal[n] + inc_horizontal_pos;
                if (array_increment_pos[n] > ((window.innerWidth + 100) / 2)) {
                    array_increment_pos[n] = 0;
                    array_size_pict[n] = size_pict_ini_val;
                    array_inc_space_tmp[n] = 0;
                    array_increment_horizontal[n] = 0;
                }
                for (var i = 1; i <= num_of_picts; i++) {
                    ctx.drawImage(idols_picts[n], array_increment_pos[n], 0, array_size_pict[n], array_size_pict[n]);
                    ctx.beginPath();
                    //ctx.arc(0,radius,size,0,2*Math.PI,false);
                    // let degrees = 270;
                    // ctx.rotate(degrees*Math.PI/180);
                    //ctx.save();
                    //var time = new Date();
                    //ctx.rotate((2*Math.PI/num_of_picts)+((2*Math.PI)/60)*time.getSeconds() + ((2*Math.PI)/60000)*time.getMilliseconds());
                    let rotation = 2 * Math.PI / num_of_picts;
                    //rotation = rotation + array_increment_horizontal[n];
                    ctx.rotate(rotation);
                }
            }



            //layer 2
            // if (incr_total2 > 300)
            // {
            //     for (var i=1; i <=maxCircle; i++){
            //     ctx.drawImage(idol2,incr_total2,0,incr_total3,incr_total3);
            //     ctx.beginPath();
            //     ctx.arc(0,radius,size,0,2*Math.PI,false);
            //     ctx.rotate(2*Math.PI/maxCircle);
            //     //ctx.fill();
            // }

            // }


            // La tierra
            // let rot_speed = 2;
            // var rad = Math.PI/180;
            // var angulo = 5;
            //console.log(time.getSeconds());
            //ctx.rotate(rad * angulo);
            //ctx.rotate( ((rot_speed*Math.PI)/60)*time.getSeconds() + ((rot_speed*Math.PI)/60000)*time.getMilliseconds() );
            //ctx.translate(incr_total,0);
            //incr_total = incr_total + incr;
            //ctx.fillRect(0,-12,50,24); // Sombra
            //ctx.drawImage(idol1,0,0);

            //   // La luna
            //var time = new Date();
            //ctx.rotate( ((2*Math.PI)/60)*time.getSeconds() + ((2*Math.PI)/60000)*time.getMilliseconds() );
            //ctx.translate(window.innerWidth /2 ,innerHeight/2);
            //ctx.drawImage(moon,-3.5,-3.5);

            // ctx.restore();

            // ctx.beginPath();
            // ctx.arc(150,150,105,0,Math.PI*2,false); // Órbita terrestre
            // ctx.stroke();

            //ctx.drawImage(sun,0,0,300,300);

            window.requestAnimationFrame(draw);
        }

        init();

    };
    // var canvas = document.getElementById('viewport'),
    // context = canvas.getContext('2d');

    // canvas.width = window.innerWidth;
    // canvas.height = window.innerHeight;
    // make_base();

    // function make_base()
    // {
    // base_image = new Image();
    // base_image.src = 'img/img2.gif';
    // base_image.onload = function(){
    //     context.drawImage(base_image, 0, 0);
    // }
    // }



</script>

</html>