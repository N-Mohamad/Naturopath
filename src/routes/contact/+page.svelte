<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w==" crossorigin="anonymous" referrerpolicy="no-referrer" />

</head>

<script>

    let nom;
    let sujet;
    let mail
    let numero
    let message

	import { prevent_default } from "svelte/internal";

</script>

<div class="container">
<div class="right-container">
    <h1>Book Free Discovery Call</h1>
    <hr>
    <p>Book in a FREE discovery call to see how we could work together , please drop me a message and I will reply shortly.
</p>
        <p> I look forward to hearing from you !</p>
        <form on:submit|preventDefault={validateForm}>
            <input type="text" placeholder="Votre nom" bind:value={nom} />
            <br /><br />
            <input type="text" placeholder="sujet" bind:value={sujet} />
            <br /><br />
            <input type="email" placeholder="Votre Mail" bind:value={mail} />
            <br /><br />
            <input type="text" placeholder="Votre Numéro" bind:value={numero} />
            <br /><br />
            <textarea class="field" placeholder="Votre Message" bind:value={message}></textarea>
            <br /><br />
            <div class="center">
            <input class="submit" type="submit" value="Envoyer message" />
            <p id="reussite"></p>
            </div>
        </form>
</div>
<div class="image-column">
    <img src="https://www.emmamoorbynd.com/wp-content/uploads/bb-plugin/cache/ezgif.com-gif-maker2-1-1536x1536-square.jpg"  alt="image">

    <div>
        <span class="fa-solid fa-phone" style="font-size: 36px; margin-right: 10px;"></span>
        <span>0000000000000</span></div>
        <br>
        <div>
        <span class="fa-solid fa-at" style="font-size: 36px; margin-right: 10px;"></span>
        <span> EMAIL ME <br>
            <a href="#">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; ############@gmail.com</a></span></div><br>
        <p>Explore our services today and follow us on Facebook for the latest news here.</p>
    </div>
</div>



    <style>
        .container {
    display: flex;
    flex-direction: row;
    width: 1200px;
    margin: 0 auto;
    padding: 20px;
}

.right-container{

        width: 50%;
        height: 100%;
        padding: 20px;
        margin: 0 auto;
        border: black;
        box-shadow:0 0 5px  ;
}
form{
        background-color: white;
        padding: 20px;
        box-sizing: border-box;
        

    }
    input, textarea{
        width: 100%;
        padding: 20px;
        box-sizing: border-box;
        outline: none;
        resize: none;
        background-color: #f7f3f3;
        border: #535555;
        
        
    }
    .center{
        text-align: left;
        width: 40%;
        border-radius: 40px ;
    }
    .field{
        height: 170px;
    }
    .submit{
        border-radius: 22px;
        background-color: #8fab72;
        border: none;
        width: 220px;
        height: 40px;
        padding: 5px;
        color: white;
    }
.image-column {
    width: 50%;
    padding-right: 50px;
    order: -1;


}
img {
    width: 100%;
    height: auto;
}
hr{
    width: 30%;
    margin-left: 0;

}
h1{
    padding-left: 20px;
    font-family: 'Poppins', sans-serif;
    font-weight: 300;
    color: #535555;
    line-height: 1.2;
}
p{
    padding-left: 20px;
    font-weight: 300;
    color: #535555;
    line-height: 1.2;
}
.fa-solid {
    margin-right: 10px;
    vertical-align: middle;
    color: rgb(107, 139, 120);
}
a{
    text-decoration: none;
    color: #8fab72;
}
</style>
