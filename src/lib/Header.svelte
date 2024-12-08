<script>
    import Logo from '$lib/Images/logo.png'
</script>

<header>
    <img src={Logo} alt="Logo" height=80>
    <ul>
        <li>Home</li>
        <li>About</li>
        <li>Services</li>
        <li>Contact</li>
        <li>Status</li>
        <li>Help</li>
    </ul>  
</header>

<style>
    header{
        padding: 1em;
        align-items: center;
        justify-content: center;
        gap: 10em;
        color:rgb(6, 4, 43);
    }
    header, ul{
        display: flex;
    }
    ul{
        list-style: none;
        padding: 1em;
        gap: 1.5em;
    }
    ul li{
        padding: 0.5em;
        background-color: white;
        border-radius: 0.4em;
        transition: background-color 0.4s, transform 0.4s;
    }
    /*Hover effect for nav items*/
    ul li:hover{
        background-color:rgb(6, 4, 43);
        color: white;
    }

    /* Keyframes for the drop effect */
    @keyframes dropIn {
        0% {
            opacity: 0;
            transform: translateY(-20px);
        }
        100% {
            opacity: 1;
            transform: translateY(0);
        }
    }

    /* Apply the dropIn animation to each item with a staggered delay */
    img{
        animation: dropIn 0.5s ease forwards;
        opacity: 0;  
    }    
    ul li {
        animation: dropIn 0.5s ease forwards;
        opacity: 0;
    }
    ul li:nth-child(1) {
        animation-delay: 0.1s;
    }
    ul li:nth-child(2) {
        animation-delay: 0.2s;
    }
    ul li:nth-child(3) {
        animation-delay: 0.3s;
    }
    ul li:nth-child(4) {
        animation-delay: 0.4s;
    }
    ul li:nth-child(5) {
        animation-delay: 0.5s;
    }
    ul li:nth-child(6) {
        animation-delay: 0.6s;
    }
</style>