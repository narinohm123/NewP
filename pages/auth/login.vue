<template>
<div class="container max-w-md mx-auto xl:max-w-3xl h-full flex bg-white rounded-lg shadow overflow-hidden">

    <div>
        <v-dialog v-model="dialog" scrollable fullscreen persistent :overlay="false" max-width="500px" transition="dialog-transition">

            <div class="col-md-6 d-none d-md-flex " style="background-color:#F1F2F1;position: relative; display: flex; flex-direction: column; justify-content: center;">
                <div class="d-flex align-items-center " style="position: relative; left:65px;">
                    <div>
                        <div>
                            <img src="@/assets/logo.png" class="Imgict">
                        </div>
                    </div>
                    <div class="d-flex flex-column ">
                        <div style="position: relative; left:-120px; top:105px; width: 27vw;">
                            <p class="Hedone">ระบบฐานข้อมูลบุคลากร</p>
                            <p class="Hedtwo">เพื่อสนับสนุนการวางแผนพัฒนาบุคลากร</p>
                            <p class="Hedthee">คณะเทคโนโลยีสารสนเทศและการสื่อสาร มหาวิทยาลัยพะเยา</p>
                        </div>
                    </div>
                </div>

            </div>
            <div class="w-full xl:w-1/2 p-8" style="background: white; display: flex; flex-direction: column; justify-content: center;">

                <form method="post" action="#" onSubmit="return false">
                    <h1 class=" text-2xl font-bold" style="display: flex; justify-content: center;">Sign in to your account</h1>

                    <div class="mb-5 mt-6">
                        <div class="bg-white shadow-md rounded px-8 pt-6 pb-8 mb-4 flex flex-col">
                            <div class="mb-4">
                                <label class="block text-grey-darker text-sm font-bold mb-2" for="username">
                                    Username
                                </label>
                                <input class="shadow appearance-none border rounded w-full py-2 px-3 text-grey-darker " id="username" type="text" placeholder="Username">
                            </div>
                            <div class="mb-6">
                                <label class="block text-grey-darker text-sm font-bold mb-2" for="password">
                                    Password
                                </label>
                                <input class="shadow appearance-none border border-red rounded w-full py-2 px-3 text-grey-darker mb-3" id="password" type="password" placeholder="******************">
                                <!-- <p class="text-red text-xs italic">Please choose a password.</p> -->
                            </div>
                            <div class="flex items-center justify-between">

                                <div class="flex items-center">
                                    <input id="remember_me" name="remember_me" type="checkbox" class="h-4 w-4 bg-indigo-500 focus:ring-indigo-400 border-gray-300 rounded">
                                    <label for="remember_me" class="ml-2 block text-sm text-gray-900">
                                        Remember me
                                    </label>
                                </div>

                            </div>
                            <div class="flex w-full mt-8">
                                <v-btn elevation="2" large x-large>Login</v-btn>
                            </div>
                        </div>

                    </div>
                </form>
            </div>

        </v-dialog>

    </div>

</div>
</template>

<script>
export default {
    data() {
        return {
            dialog: true
        }
    }
}
</script>

<style>
.Imgict {
    width: 65%;
    position: relative;
    top: -60px;
}

.Hedone {
    position: relative;
    font-size: 2.8em;
    top: 10px;
    color: #7030A0;
}

.Hedtwo {
    position: relative;
    top: -10px;
    font-size: 1.7em;
    color: #7030A0;
}

.Hedthee {
    position: relative;
    top: -25px;
    font-size: 1.3em;
    color: #C55A11;
}
</style>
