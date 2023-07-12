<template>
    <div class="container">
        <article>
            <h2>CONTACT US</h2>
            <div class="row">
                <div class="container-lg form">
                    <form @submit="validateForm">
                        <div class="row">
                            <label for="name">Name</label><br>
                            <input type="text" id="name" v-model="name" :class="{ errora: errors.name }" /><br>
                            <span v-if="errors.name" class="error">{{ errors.name }}</span>
                        </div><br>

                        <div class="row">
                            <label for="email">Email</label>
                            <input type="email" id="email" v-model="email" :class="{ errora: errors.email }" />
                            <span v-if="errors.email" class="error">{{ errors.email }}</span>
                        </div><br>
                        <div class="row">
                            <label for="password">Message</label>
                            <textarea name="" cols="30" rows="10" id="message" v-model="message"
                                :class="{ errora: errors.message }"></textarea>
                            <span v-if="errors.message" class="error">{{ errors.message }}</span>
                        </div>
                        <br>
                        <div class="row">
                            <button class="btnsub" type="submit">Submit</button>
                        </div>
                    </form>
                </div>
            </div>
        </article>
    </div>
    <div>

    </div>
</template>
  
<script>
export default {
    data() {
        return {
            name: "",
            email: "",
            message: "",
            errors: {}
        };
    },
    methods: {
        validateForm(event) {
            this.errors = {};

            if (!this.name) {
                this.errors.name = "This field is required.";
            }

            if (!this.email) {
                this.errors.email = "Invalid email address.";
            } else if (!this.isValidEmail(this.email)) {
                this.errors.email = "Invalid email address.";
            }

            if (!this.message) {
                this.errors.message = "This field is required.";
            }

            if (Object.keys(this.errors).length === 0) {
                // Form is valid, submit the data
                // You can perform your desired action here, like sending the form data to the server
                console.log("Form submitted");
            }

            event.preventDefault();
        },
        isValidEmail(email) {
            // Simple email validation regex
            const emailRegex = /\S+@\S+\.\S+/;
            return emailRegex.test(email);
        }
    }
};
</script>
  
<style scoped>
h2 {
    text-align: center;
    margin-top: 90px;
    margin-bottom: 40px;
    font-size: 26px;
    font-weight: bold;
}

.form {
    padding-left: 20vw;
    padding-right: 20vw;
}

.error {
    color: red;

}

.errora {
    border: 1px solid #ff0000;

}

.btnsub {
    width: 100%;
    background-color: rgb(0, 132, 255);
    color: #ffffff;
    font-size: 18px;
    font-weight: bold;
    border: none;
    padding: 5px;
}
</style>
  