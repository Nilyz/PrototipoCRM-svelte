<script>
    import Button from "../lib/Button.svelte";
    import Toggle from "../lib/Toggle.svelte";
    import ArrowBtn from "../lib/ArrowBtn.svelte";
    import Input from "../lib/Input.svelte";
</script>

<main>
    <div class="arrowBtnCont">
        <ArrowBtn path="/"/>
    </div>
    <div class="loginTextCont">
        <h1>Iniciar Sesión</h1>
    <p>Inicia sesión con el correo de la empresa para poder acceder</p>
    </div>
    <div class="loginFormCont">
        <div class="inputCont">
            <Input typeText="text" placeholder="correo@gmail.com"/>
        <Input typeText="password" placeholder="contraseña"/>
        </div>
        <a class="forgot" href="">¿Olvidastes la contraseña?</a>
        <Button btnText="Iniciar Sesión" btnWidth=70%/>
        <div class="rememberMeCont">
            <p>Recuérdame</p>
            <Toggle/>
        </div>

    </div>
</main>

<style>
    main {
        height: 100vh;
        background-color: var(--color-brown);
        color: var(--color-cream);
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-direction: column;
    }
    a{
        color: var(--color-darkBrown);
        font-size: 14px;
        width: 70%;
        text-align: right;
    }
    .arrowBtnCont{
        width: 100%;
        align-items: start;
        display: flex;
        justify-content: start;
        margin-top: 50px;
    }
    .loginTextCont{
        margin-bottom: 80px;
    }
    h1{
        font-size: 40px;
    }
    p{
        font-size: 22px;
        padding: 20px 30px 20px 30px;
    }
    .loginFormCont{
        height: 55%;
        width: 100%;
        background-color: var(--color-cream);
        border-radius: 60px 60px 0px 0px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        color: var(--color-darkBrown);
        padding: 10% 0;
    }
    .inputCont{
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        gap: 25px;
        margin-bottom: 20px;
    }
    .forgot{
        margin-bottom: 40px;
    }
    .rememberMeCont{
        width: 70%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-top: 20px;
    }
    .rememberMeCont p{
        font-size: 18px;
        padding: 0;
    }
</style>
