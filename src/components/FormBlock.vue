<template>
  <div
    class="min-h-screen bg-[url('../assets/img/form-bg.svg')] bg-cover pt-5 pb-10 px-5"
  >
    <div class="max-w-[1200px] mx-auto">
      <form
        ref="form"
        @submit.prevent="submitForm"
        class="pt-24 flex flex-col items-center"
      >
        <div class="text-center">
          <h2
            class="text-[50px] text-white font-[700] max-[630px]:text-[40px] max-[470px]:text-[32px]"
          >
            Оставьте заявку
          </h2>
          <span
            class="text-[22px] text-[#D2D2D2] font-[400] max-[630px]:text-[19px] max-[470px]:text-[15px]"
            >и наши менеджеры свяжутся с вами в ближайшее время</span
          >
        </div>
        <div class="grid gap-4 grid-cols-2 w-full max-[470px]:grid-cols-1">
          <div class="mt-20 flex flex-col items-start max-[470px]:mt-5">
            <span class="text-red-500 text-[14px]">{{
              this.formValue.errors.name
            }}</span>
            <input
              v-model.trim="formValue.name"
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите имя"
            />
            <span class="text-red-500 text-[14px]">{{
              this.formValue.errors.number
            }}</span>
            <input
              v-model.trim="formValue.number"
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите телефон"
            />
            <input
              v-model.trim="formValue.extrafield"
              type="text"
              class="w-[70%] border-b focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:w-[85%]"
              placeholder="Дополнительные данные"
            />
          </div>
          <div class="mt-20 flex flex-col items-end max-[470px]:mt-0">
            <span class="text-red-500 text-[14px]">{{
              this.formValue.errors.email
            }}</span>
            <input
              v-model.trim="formValue.email"
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите E-mail"
            />
            <select
              v-model="formValue.questions"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
            >
              <option class="text-black" value="вопроса 0">Тема вопроса</option>
              <option class="text-black" value="вопроса 1">вопроса 1</option>
              <option class="text-black" value="вопроса 2">вопроса 2</option>
              <option class="text-black" value="вопроса 3">вопроса 3</option>
            </select>

            <div class="">
              <div class="flex flex-col mb-2">
                <span class="text-red-500 text-[14px]">{{
                  this.formValue.errors.personalData
                }}</span>
                <div class="flex items-center">
                  <input
                    type="checkbox"
                    id="chek-1"
                    class="bg-inherit mr-5"
                    v-model="formValue.rules.personalData"
                  />
                  <label
                    class="text-white text-[13px] font-[400] max-[470px]:text-[10px]"
                    for="chek-1"
                    >Я соглашаюсь на обработку моих персональных данных</label
                  >
                </div>
              </div>

              <div class="flex flex-col mb-2">
                <span class="text-red-500 text-[14px]">{{
                  this.formValue.errors.politics
                }}</span>
                <div class="flex items-center">
                  <input
                    type="checkbox"
                    id="chek-2"
                    class="bg-inherit mr-5"
                    v-model="formValue.rules.politics"
                  />
                  <label
                    class="text-white text-[13px] font-[400] max-[470px]:text-[10px]"
                    for="chek-2"
                    >Я соглашаюсь с политикой конфиденциальности</label
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
        <button
          type="submit"
          class="text-white w-full max-w-[350px] py-3.5 mt-16 bg-[#ee3e53] text-[22px] font-[500] text-center rounded-3xl cursor-pointer hover:bg-[#fa5598] transition-colors duration-200 ease-in-out max-[1470px]:text-[20px] max-[1470px]:py-2.5 max-[1470px]:max-w-[250px] max-[400px]:text-[16px] max-[400px]:max-w-[200px] max-[610px]:mt-8"
        >
          Оставить заявку
        </button>
      </form>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      formValue: {
        errors: {
          name: "",
          email: "",
          number: "",
          politics: "",
          personalData: "",
        },
        name: "",
        email: "",
        number: "",
        extrafield: "",
        questions: "вопроса 0",
        rules: {
          politics: false,
          personalData: false,
        },
      },
    };
  },

  methods: {
    submitForm(e) {
      const emailValid =
        /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;

      let isEmailValid = emailValid.test(this.formValue.email);

      if (!this.formValue.name) {
        this.formValue.errors.name = "Name is required";
      } else {
        this.formValue.errors.name = "";
      }

      if (!this.formValue.email) {
        this.formValue.errors.email = "Email is required";
      } else {
        this.formValue.errors.email = "";
      }
      if (!isEmailValid) {
        this.formValue.errors.email = "Email must be correct";
      } else {
        this.formValue.errors.email = "";
      }

      if (this.formValue.number == "") {
        this.formValue.errors.number = "Number is required";
      } else {
        this.formValue.errors.number = "";
      }
      if (this.formValue.number.length <= 10) {
        this.formValue.errors.number = "Number must be more than 10";
      } else {
        this.formValue.errors.number = "";
      }

      if (!this.formValue.rules.politics) {
        this.formValue.errors.politics = "This field is required";
      } else {
        this.formValue.errors.politics = "";
      }

      if (!this.formValue.rules.personalData) {
        this.formValue.errors.personalData = "This field is required";
      } else {
        this.formValue.errors.personalData = "";
      }

      if (
        !this.formValue.errors.email &&
        !this.formValue.errors.name &&
        !this.formValue.errors.number &&
        !this.formValue.errors.personalData &&
        !this.formValue.errors.politics
      ) {
        this.fetchForm(this.formValue);
      }
    },

    async fetchForm(values) {
      let url = ``;

      // const response = await axios.post(url, values);
      // console.log("response", response);
    },
  },
  mounted() {
    this.$emit("addFormRef", this.$refs.form);
  },
};
</script>
