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
        background-color: greenyellow;
        align-items: center;
    }
    img{
        border: 3px solid red;
    }
    header, ul{
        display: flex;
    }
    ul{
        background-color: red;
        list-style: none;
        padding: 1em;
        gap: 0.5em;
    }
    ul li{
        padding: 0.5em;
        background-color: white;
    }
</style>