<template >
    <div class="contact">
        <form action="https://formspree.io/f/xvoyqypq" method="post">
            <label for="">Name</label><br>
            <input type="text" name="name" placeholder="Enter your name" required><br>
            <label for="">Surname</label><br>
            <input type="text" name="surname" placeholder="Enter your surname" required><br>
            <label for="">Email Address</label><br>
            <input type="email" name="email" placeholder="Enter your email address" required><br>
            <label for="">Contact Details</label><br>
            <input type="number" name="contact" placeholder="Enter your contact no." required><br>
            <label for="">Message</label><br>
            <input class="msg" type="text" name="message" placeholder="Enter your message"><br>
            <button>SUBMIT</button>
        </form>
        <div class="info">
        <a href=""><i class="fa-sharp fa-solid fa-envelope-open" style="color:black;" > dywiliuzukhanye@gmail.com</i></a><br>
        <br>
        <a href=""><i class="fa-solid fa-phone " style="color:black;" > 073 601 8746</i></a> <br>
    </div>
    </div>
</template>
<style scoped>
.contact{
    display: flex;
}
form{
    padding: 2rem;
}
input{
    width: 40rem;
   
}
input[type="number"]::-webkit-inner-spin-button,
.input[type="number"]::-webkit-outer-spin-button{
    -webkit-appearance:none ;
   
}
label{
    color: black;
    font-style: italic;
    font-weight: bold;
}
.msg{
    height: 10rem;
}
.info{
    margin: 10rem;
    font-size: 1.2rem;
    color: black;
    
    }
    button{
margin: 2rem;
width: 7rem;
background-color: plum;
border: solid plum;
    }
 

    
</style>