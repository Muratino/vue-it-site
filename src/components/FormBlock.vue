<template>
  <div
    class="min-h-screen bg-[url('../assets/img/form-bg.svg')] bg-cover pt-5 pb-10 px-5"
  >
    <div class="max-w-[1200px] mx-auto">
      <form class="pt-24 flex flex-col items-center">
        <div class="text-center">
          <h2 class="text-[50px] text-white font-[700] max-[630px]:text-[40px] max-[470px]:text-[32px]">Оставьте заявку</h2>
          <span class="text-[22px] text-[#D2D2D2] font-[400] max-[630px]:text-[19px] max-[470px]:text-[15px]"
            >и наши менеджеры свяжутся с вами в ближайшее время</span
          >
        </div>
        <div class="grid gap-4 grid-cols-2 w-full max-[470px]:grid-cols-1">
          <div class="mt-20 flex flex-col items-center max-[470px]:mt-5">
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите имя"
            />
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите телефон"
            />
            <input
              type="text"
              class="w-[70%] border-b focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:w-[85%]"
              placeholder="Введите сообщение"
            />
          </div>
          <div class="mt-20 flex flex-col items-center max-[470px]:mt-0">
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
              placeholder="Введите E-mail"
            />
            <select
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2 max-[470px]:mb-6 max-[470px]:w-[85%]"
            >
              <option class="text-black" disabled value="0">Тема вопроса</option>
              <option class="text-black" value="1">вопроса 1</option>
              <option class="text-black" value="2">вопроса 2</option>
              <option class="text-black" value="3">вопроса 3</option>
            </select>

            <div class="">
              <div class="flex items-center mb-2">
                <input type="checkbox" id="chek-1" class="bg-inherit mr-5" />
                <label class="text-white text-[13px] font-[400] max-[470px]:text-[10px]" for="chek-1"
                  >Я соглашаюсь на обработку моих персональных данных</label
                >
              </div>

              <div class="flex items-center">
                <input type="checkbox" id="chek-2" class="bg-inherit mr-5" />
                <label class="text-white text-[13px] font-[400] max-[470px]:text-[10px]" for="chek-2"
                  >Я соглашаюсь с политикой конфиденциальности</label
                >
              </div>
            </div>
          </div>
        </div>
        <button
          class="text-white w-full max-w-[350px] py-3.5 mt-16 bg-[#ee3e53] text-[22px] font-[500] text-center rounded-3xl cursor-pointer hover:bg-[#fa5598] transition-colors duration-200 ease-in-out max-[1470px]:text-[20px] max-[1470px]:py-2.5 max-[1470px]:max-w-[250px] max-[400px]:text-[16px] max-[400px]:max-w-[200px] max-[610px]:mt-8"
        >
          Оставить заявку
        </button>
      </form>
    </div>
  </div>
</template>
