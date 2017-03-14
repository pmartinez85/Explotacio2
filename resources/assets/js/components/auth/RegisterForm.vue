<template>

    <form method="post" @submit.prevent="submit">
        <div class="form-group has-feedback">
            <input type="text" class="form-control" placeholder="Put your name here" name="name" value=""/>
            <span class="glyphicon glyphicon-user form-control-feedback"></span>
        </div>

        <div class="form-group has-feedback">
            <input type="text" class="form-control" placeholder="Put your username here" name="username"/>
            <span class="glyphicon glyphicon-user form-control-feedback"></span>
        </div>


        <div class="form-group has-feedback">
            <input type="email" class="form-control" placeholder="Put your email" name="email" value=""/>
            <span class="glyphicon glyphicon-envelope form-control-feedback"></span>
        </div>
        <div class="form-group has-feedback">
            <input type="password" class="form-control" placeholder="Put your password here" name="password"/>
            <span class="glyphicon glyphicon-lock form-control-feedback"></span>
        </div>
        <div class="form-group has-feedback">
            <input type="password" class="form-control" placeholder="Confirmation Here" name="password_confirmation"/>
            <span class="glyphicon glyphicon-log-in form-control-feedback"></span>
        </div>
        <div class="row">
            <div class="col-xs-1">
                <label>
                    <div class="checkbox_register icheck">
                        <label>
                            <input type="checkbox" name="terms">
                        </label>
                    </div>
                </label>
            </div><!-- /.col -->
            <div class="col-xs-6">
                <div class="form-group">
                    <button type="button" class="btn btn-block btn-flat" data-toggle="modal" data-target="#termsModal">Terms & Cond</button>
                </div>
            </div><!-- /.col -->
            <div class="col-xs-4 col-xs-push-1">
                <button type="submit" class="btn btn-primary btn-block btn-flat">Submit</button>
            </div><!-- /.col -->
        </div>
    </form>

</template>
<style>
    body{
        background-color:#ff0000;
    }
</style>
<script>
    export default {
        mounted() {
            console.log('Component register-form mounted.')
        },
        methods: {
            submit() {
            console.log('submiting')
            }
        },

    }

</script>
