<script>
  import Header from "../Header.svelte";
  import gradphoto from "$lib/images/grad1.jpeg"
</script>

<html class="no-js" lang="en">
    <head>
        <title>About Me</title>
        <meta charset="UTF-8">
        <meta name="description" content="A little bit of background about me" >
        <meta name="keywords" content="Adam,Bauer,background,about,travel,computer,engineer,engineering" >
        <meta name="author" content="Adam Bauer" >
        <meta name="viewport" content="width=device-width">
        
    </head>
    <body>
    <header>
        <h1>
            <span class="underline-container">
                Hi, I'm <span>Adam</span>
              </span>
              </h1>
    </header>

    


   
    <noscript><p>JavaScript is currently disabled</p></noscript>
   
<main id="about">

    <section>
    
        <div class="about-box" >
       
            <!--img class="img-slide-right" src="src/li/images/grad1.jpeg" alt="Graduation" title="Graduation photo. Onto the next chapter"-->
            <!--img class="slide-in-from-left" src={gradphoto} alt="Graduation" title="Graduation photo. Onto the next chapter"-->
            <img src={gradphoto} alt="Graduation" title="Graduation photo. Onto the next chapter">


        <div class="about-text-div">
        <p class="right-text"> 
        For as long as I can remember, I've always wanted to build things. I always had this nagging question of wanting to know how technology works so that I could fulfill this desire to build and innovate. Now, as a recent graduate with a B.S in Computer Engineering from UCSD's Jacobs School of Engineering, I'm excited to fulfill this dream
        as I move forward into the next chapters. 
        </p>
        <p id="right-text2">
			I've had the pleasure to work alongside classmates and engineers from various backgrounds and learn how to be a team player. 
            Within my free time, I joined Rocket Propulsion Laboratory (RPL), an organization of engineers sponsered by Collins Aerospace and Blue Origin 
            with the goal to build rocketry. I worked as a software member on the Avionics team, and had the pleasure to learn how to work alongside
            other different engineers to fulfill their software needs. I'm grateful for this time, as I was able to develop communication skills
            of working with engineers from different majors and backgrounds.
        </p>

        <p id="text3-start">
            My remaining free time was spent towards Camp Kesem, a nation wide organization that helps provide support for children whose family members
            deal with cancer.
            I was lucky enough to work with some amazing kids, and even got to see them grow up over the years. 
            Within all the decisions of my college career, and possibly my life, this volunteer work serves as one the best decisions I've ever made. 

            </p>
        </div>
        
            <p id="text3-end" hidden>
                Within all the decisions of my college career, and possibly my life, this volunteer work serves as one the best decisions I've ever made. 
        
            </p>
    </div>

    <h2 id="education">Education</h2>
            <ul id="education-list">
                <li>B.S in Computer Engineering from UCSD</li>
                <li>Associates in Computer Science</li>
                <li>Associates in Mathematics</li>
                <li>Associates in Physics </li>
            </ul>

        <h2 id="languages-header">Languages/Tools</h2>
        <p>A brief overview of tools I've worked with, click on a term to expand. </p>
        <ul class="overview">
            <li>
                <details>
                <summary><h4 class="summary">Python</h4></summary>
                <ul>
                    <li><h4>AI Search & Reasoning </h4> Implemented AI algorithms for decision based topics such as playing 2048, Black Jack, GO, using techniques such as Monte Carlo Tree Search, A* and Reinforcement Learning.  </li>
                    <li><h4>ML Recommender Systems </h4> Implemented ML methodologies ranging to provide as movie & product recommendations using various ML techniques</li>
                    <li><h4>Web Scraping/Interactions</h4> Implemented programs using towards retrieving and cleaning data using PANDAS and other data science based libraries. 
                         </li>
                </ul>
               
            </details>
            </li>
            <li>
            <details><summary><h4 class="summary">Java</h4></summary>
               <ul>
                <li><h4>Nachos</h4> 
                Implemented NACHOS for OS simulation.</li>
                <li><h4>Data Structures</h4>
                Base Data Structures course including sorting, tree traversals, and graphs.</li>
              <li><h4>OOP</h4> Java fundamentals including Object Oriented Programming </li>
            </ul>
            </details></li>
        <li>
            <details><summary><h4 class="summary">C++</h4></summary>
                <ul>
                    <li>
                        <h4>Advanced Data Structures</h4>
                        Topics including self balancing trees, hashing, additional tree and graph traversal techniques.
                    </li>
                    <li><h4>Huffman Encoder</h4>
                        Built a Huffman Encoder Compression program to compress file sizes. 
                    </li>
                    <li><h4>OOP</h4>
                    Fundamentals of C++, pointers,double pointers, memory management, and Objected Oriented Programming </li>
                </ul>
            </details></li>
       <li>
            <details>
                <summary>
                    <h4 class="summary">
                        C
                    </h4>
                </summary>
            <ul>
                <li>
                    <h4>Fundamentals</h4>
                    Fundamentals of C programming with some light usage alongside Arduino IDE. 
                </li>   
            </ul>
            </details>
        </li>
        <li>
            <details>
                <summary>
                    <h4 class="summary">
                        Web Development
                    </h4>
                    
                </summary>
                <ul>
                    <li>
                        <h4>HTML</h4>
                        Fundamentals of HTML including the DOM, semantic useage, and form validation.
                        This website was written by hand HTML and CSS alongside Svelte.
                    </li>
                    <li>
                        <h4>CSS</h4>
                        Likewise, the fundamentals of CSS for styling semantic HTML pages.
                        Once again, the majority of this site was done by hand with CSS. 
                    </li>

                    <li> 
                        <h4>Vanilla Javascript</h4>
                        Fundamentals of Javascript for adding interactivity to accompany a website,
                        performing form validation, performing requests. 
                    </li>
                    <li>
                        <h4>
                            Svelte
                        </h4>
                        The basics of using Svelte/Svelte Kit, including to create this website. 
                    </li>
                </ul>
            </details>

            <details>
               <summary><h4 class="summary">Git</h4></summary>
               <ul>
                <li>Worked with Github on an organizational level to interact 
                     and collaborate with other software developers to maintain 
                     our code and work together on projects </li>
               </ul>
            </details>

            <li>
                <details>
                <summary><h4 class="summary">SystemVerilog & Quartus </h4>
                </summary>
                <ul>
                    <h5>Inclusive of Simulation & Synthesis</h5>
                    <li>
                        <h4>
                            Viterbi Decoder
                        </h4> 
                        Term project involved implementing the Viterbi Decoder.
                     </li>
                    

                        <li>
                            <h4>
                                UART Receiver
                            </h4>
                            Using FSM implementation with binary state encodings for the states,
                             implemented a UART receiver.
                        </li>


                    <li>
                        <h4>
                            4 Bit Counters
                        </h4>
                    Implemented both a straight 4 bit counter and a 4 bit Johnson Counter
                    </li>
                    <li>
                        <h4> 
                            4 Bit Barrel Shifter
                        </h4>
                    Implemented a 4 bit barrel shifter with directional option bits to shift left or right. 
                    Operations included left shift, right shift, left rotate and right rotate.
                    Implemented this barrel shifter using a cascade of 2x1 MUXs. 
                  </li>
                  <li>
                    <h4>N bit LFSR</h4>
                    Implemented an N &isin; [2,8] bit LFSR using XOR implementation. 
                  </li>
                  
                  <li>
                    <h4>N Bit Rate 1/2 Convolutional Encoder</h4>
                    Implemented a N &isin; [3,9] bit parameterized 1/2 convolutional encoder
                    using XOR and ANDs
                  </li>

                  <li>
                    <h4>Gray Code to Binary Convertor </h4>
                    Implemented an N bit convertor that would take gray code as input and output its
                    equivalent value in binary. 
                  </li>
                  <li><h4>Multiplexer </h4>Implemented a 2 to 1 MUX</li>
                  <li><h4>ALU Bit Conversion</h4>Implemented a 1 bit to 4 bit ALU</li>
                </ul>


        </li>
        </ul>

        <h2 id="in-progress">In Progress</h2>
        <p class="progress-text">Here's currently some things I'm working on expanding my knowledge on or learning: 
        </p>
        <ol>
            <li>
            <h4 class="progress-subheader">Python Projects</h4> 
            <p class="progress-text">
                I'm currently expanding my usage of Python for some fun projects.
                I've been utilizing this time to learn some fun libraries and automate
                certain tasks for myself, including a desktop cleaner and a webscraper.
            </p>
        </li>


            <li>
                <h4 class="progress-subheader">Backend</h4>
                <p class="progress-text">I'm currently working on 
                    learning about Backend/Database management, particularly about using Django. 
                </p>

            </li>
            <li>
                <h4 class="progress-subheader">Arduino/Raspberry Pi</h4>
                <p class="progress-text">
                    I've been wanting to get my hands on working closer with hardware and 
                    am utilizing this time to tinker with these fun devices
                    and work on various projects. 
                </p>
            </li>
        </ol>


            

            
        
            <h2 id="courses-header">Courses</h2>
            <ul class="overview">
                <li>
                    <details> 
                        <summary>Advanced Data Structures</summary>
                        <p>C++ programming including topics: Graph Traversals, Self Balancing Trees, Tries, Fast String Searching, Hashes, Compression. Implemented both a Huffman Encoding and a Graph project. </p>

                    </details>
                </li>

				<li>
                    <details> 
                        <summary>Recommender Systems</summary>
                        <p>C++ programming to include: Graph Traversals, Trees, Fast String Searching, Hashes, Compression. Implemented both a Huffman Encoding and a Graph project. </p>

                    </details>
                </li>


				<li>
                    <details> 
                        <summary>AI</summary>
                        <p>C++ programming to include: Graph Traversals, Trees, Fast String Searching, Hashes, Compression. Implemented both a Huffman Encoding and a Graph project. </p>

                    </details>
                </li>

                <li>
                    <details> 
                        <summary>Analog Circuits</summary>
                        <p>Circuit analysis including using techniques such as Kirchoff's Laws, Thevenin and Norton theorems, Nodal analysis and more.</p>

                    </details>


                </li>
                <li>
                    <details>
                        <summary>Analog Circuits Design</summary>
                        <p>Basic proficiency in designing circuits to fulfill requirements using LTSpice. Analysis techniques of BJTs, MOSFETs, and OP Amps</p>
                    </details>
                </li>
                <li>
                    
                    <details> 
                        <summary>Signals & Systems</summary>
                        <p>Observation and focus on Fourier Series and Transforms, Laplace, filtering, discretization and recovery of signals. </p>

                    </details>

                    
                </li>
            </ul>

            


        
        <h3 id="hobbies">Hobbies</h3>
       <p>
        During my free time I enjoy lifting weights, hiking, learning guitar, watching old movies and
        spending time with my dog. I'm also a big foodie and enjoy cooking as well as discovering new spots to try different cuisines. 
        Idk insert more stuff here blah blah blah
       </p>

            

        <h3 hidden id="fun-facts">Fun Facts</h3>
        <ol hidden >
            <li>I <b>love</b> Corgis!</li>
            <li>I have a dog named Yogi</li>
            <li>I think Greek style french fries are the best version</li>
            <li>I'm trying to learn how to do a handstand</li>
            <li>The most recent concert I've been to was George Clinton</li>
            <li>The unknown depths of the ocean and its inhabitants are frightening and fascinating to me</li>
        </ol>
        

        

</main>

    </body>
</html>

<style>
/*
    h2 {
        margin-left: 2%;
    }

    h2#education{
        margin-left: 3%;
    }


h2#education {
    text-align: left;
    margin-left: 1%;
}
*/

@keyframes slideFromLeft{
    from {
        transform: translateX(-300%);
        
    } 

    to{
        transform: translateX(0);
    }
}

@keyframes littleBobble{
    from{
        transform:translateX(0) ;

    }
    to {
        transform: translateX(-10);

    }
}

@keyframes slideFromRight {
    from {
        transform: translateX(300%);
    }

    to {
        transform: translateX(0) ;
    }


}

@keyframes slideFromTop{
    from {
        transform: translateY(-300%);
    }

    to {
        transform: translateY(0) ;
    }
}

@keyframes slideFromBottom {
    from {
        transform: translateY(1000%);
    }

    to {
        transform: translateY(0) ;
    }


}

img{
    /* 
    animation: slideLeft 3s ease-in 3 3 normal forwards;
    animation: animation-name duration timing delay iteration direction
    animation-name: slideLeft;
    animation-duration: 2s;
    */
    animation: 1.3s ease-in  normal slideFromLeft,
    1.5s ease-in  normal littleBobble;

   max-width: 100%;
}

h2#education{
    text-align: left;
    margin-left: 15%;
   
}
h2 {
   text-align: center;
    margin-bottom:1% ;
    
}


p {
    margin-top : 1% ;
    margin-bottom:1%;
    animation: 1.5s ease-in  normal slideFromRight;
}

h1{
    animation: 1.2s ease-in normal slideFromTop;
}

h2,h3,h4,h5 {
    animation: 1.5s ease-in  normal slideFromLeft;
}
    


     h4{ 
        margin-bottom: 2px;
        margin-top: 2px;
        
    }
    .summary {
        display: inline;
        text-decoration: none;
       
    }

    h2#in-progress {
        text-align: center;
        margin-left: 0;
    }

    h4.progress-subheader{
        text-decoration: none;
        
    }

    ul,ol {
        animation: 1.5s ease-in  normal slideFromBottom;
    }

    p.progress-text {
        margin-top: 0;
        margin-bottom: 0px;
    }

    ul, ol {
        padding-left: 1%;
        margin-top: 1%;
    }

    .overview {
        list-style-type: none;
    }

    #education+ul{ 
        cursor: default;

    }

    h5 {
        margin: 1% 0 1% 0;
    }





    
    h3#courses-header{
        text-align: center;
    }

   
   
    
  
</style>

