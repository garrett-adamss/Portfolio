<template>
    <div class="container-fluid contact">
        <h1 class="d-flex justify-content-center p-2"><b>Contact</b></h1>
        <div class="row justify-content-center p-1">
            <img class="col-1" src="https://www.freepnglogos.com/uploads/black-email-logo-png-0.png" alt="phone">
            <h4 class="col-3">562-293-8735</h4>
        </div>
        <div class="row justify-content-center p-1">
            <img class="offset-md-3 col-md-1"
                src="https://www.pngall.com/wp-content/uploads/2016/05/Phone-Download-PNG.png" alt="email">
            <h4 class="col-md-6">garrettadams27@gmail.com</h4>
        </div>
        <form>
            <div class="d-flex justify-content-center p-1">
                <input class="form-size" type="text" id="name" name="name" placeholder="Email">
            </div>
            <div class="d-flex justify-content-center p-1">
                <textarea class="form-size" type="email" id="message" name="message" placeholder="Message" maxlength="500"></textarea>
            </div>
            <div class="d-flex justify-content-center p-1">
                <button class="btn btn-outline-secondary" type="submit">submit</button>
            </div>
        </form>
    </div>
</template>


<script>
export default {
    setup() {

        return {

        }
    }
}
</script>


<style lang="scss" scoped>
.contact{ 
    min-height: 80vh;
}
img {
    height: 2.3em;
    object-fit: scale-down;
    object-position: center;
}
input[type=text]:focus {
  border: 3px solid #555;
}
.form-size{
    width: 43%;
}
textarea{
    resize: none;
}
</style>