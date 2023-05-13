<template>
  <div class="w-full h-screen bg-[url('../assets/img/form-bg.svg')] bg-cover">
    <div class="max-w-[1200px] mr-auto ml-auto">
      <form class="pt-24">
        <div class="text-center">
          <h2 class="text-[50px] text-white font-[700]">Оставьте заявку</h2>
          <span class="text-[22px] text-[#D2D2D2] font-[400]"
            >и наши менеджеры свяжутся с вами в ближайшее время</span
          >
        </div>
        <div class="grid gap-4 grid-cols-2">
          <div class="mt-20">
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2"
              placeholder="Введите имя"
            />
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2"
              placeholder="Введите телефон"
            />
            <input
              type="text"
              class="w-[70%] border-b focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2"
              placeholder="Введите сообщение"
            />
          </div>
          <div class="mt-20">
            <input
              type="text"
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2"
              placeholder="Введите E-mail"
            />
            <select
              class="w-[70%] border-b mb-16 focus:outline-none bg-inherit text-white text-[15px] font-[400] py-2"
            >
              <option class="text-black" value="0">Тема вопроса</option>
              <option class="text-black" value="1">вопроса 1</option>
              <option class="text-black" value="2">вопроса 2</option>
              <option class="text-black" value="3">вопроса 3</option>
            </select>

            <div class="flex items-center mb-2">
              <input type="checkbox" id="chek-1" class="bg-inherit mr-5" />
              <label class="text-white text-[13px] font-[400]" for="chek-1"
                >Я соглашаюсь на обработку моих персональных данных</label
              >
            </div>
            <div class="flex items-center">
              <input type="checkbox" id="chek-2" class="bg-inherit mr-5" />
              <label class="text-white text-[13px] font-[400]" for="chek-2"
                >Я соглашаюсь с политикой конфиденциальности</label
              >
            </div>
          </div>
        </div>

        <div class="mt-40 flex items-center justify-center">
          <button
            class="text-white w-[351px] h-[72px] bg-[#ee3e53] text-[22px] font-[500] text-center rounded-3xl cursor-pointer hover:bg-[#fa5598] transition-colors duration-200 ease-in-out"
          >
            Оставить заявку
          </button>
        </div>
      </form>
    </div>
  </div>
</template>
