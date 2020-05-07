<template>
    <div>
        <h1 class="statement">Contact Us</h1>
        <p class="bodytext"></p>
        <form>
            <div class="form-group">
                <label for="exampleFormControlInput1">Email address</label>
                <input type="email" class="form-control" id="exampleFormControlInput1" placeholder="example@yourcompany.com">
            </div>
            <div class="form-group">
                <label for="exampleFormControlSelect1">Gender</label>
                <select class="form-control" id="exampleFormControlSelect1">
                    <option>Male</option>
                    <option>Female</option>
                </select>
            </div>
            <div class="form-group">
                <label for="exampleFormControlSelect2">Country</label>
                <select multiple class="form-control" id="exampleFormControlSelect2">
                    <option>USA</option>
                    <option>Canada</option>
                    <option>Mexico</option>
                    <option>Spain</option>
                    <option>Germany</option>
                </select>
            </div>
            <div class="form-group">
                <label for="exampleFormControlTextarea1">Write a message</label>
                <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
            </div>
        </form>
        <nuxt-link to="/" class="callToAction">Go Back</nuxt-link>
    </div>
</template>