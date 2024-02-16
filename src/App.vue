<template>
  <div class="bg-transparent w-full">
    <div class="bg-white p-2 mt-3">
      <div class="flex gap-4 items-center">
        <CustomInput
          placeholder="Find a product"
          customClass="w-3/4 flex bg-white border text-sm px-3 py-2 rounded border-[#E0E2E4"
        />
        <CustomButton
          customClass="w-1/4 px-3 text-sm rounded text-white py-2 bg-[#375673]"
        >
          Search
        </CustomButton>
      </div>

      <div class="flex gap-4 items-center mt-4">
        <CustomInput
          placeholder="Product Name"
          customClass="flex-1 flex bg-white text-sm border px-3 py-2 rounded border-[#E0E2E4"
        />
        <CustomButton
          customClass=" flex-none px-3 text-sm rounded text-white py-2 bg-[#375673]"
        >
          Add Product
        </CustomButton>
      </div>

      <div class="flex flex-col gap-4">
        <ListItem
          :date="item.date"
          :name="item.name"
          :key="index"
          v-for="(item, index) in data"
          :src="item.image"
        />
      </div>
    </div>

    <div class="flex justify-between items-center px-2 text-sm text-[#252526]">
      <p>
        page <span class="font-bold">1</span> of
        <span class="font-bold">2</span>
      </p>

      <p>Sort by <span class="font-bold">Sort order</span></p>

      <div class="flex items-center gap-1">
        <span>10</span>
        <span>
          <svg
            width="16"
            height="16"
            viewBox="0 0 16 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M12.4714 5.47133C12.3463 5.34635 12.1768 5.27614 12 5.27614C11.8233 5.27614 11.6537 5.34635 11.5287 5.47133L8.47136 8.52866C8.34461 8.65032 8.17572 8.71826 8.00003 8.71826C7.82434 8.71826 7.65545 8.65032 7.52869 8.52866L4.47136 5.47133C4.34563 5.34989 4.17722 5.28269 4.00243 5.28421C3.82763 5.28573 3.66042 5.35584 3.53682 5.47945C3.41321 5.60306 3.3431 5.77026 3.34158 5.94506C3.34006 6.11986 3.40726 6.28826 3.52869 6.414L6.58536 9.47133C6.77108 9.65708 6.99158 9.80443 7.23425 9.90496C7.47692 10.0055 7.73702 10.0572 7.99969 10.0572C8.26237 10.0572 8.52247 10.0055 8.76514 9.90496C9.00781 9.80443 9.22831 9.65708 9.41403 9.47133L12.4714 6.414C12.5963 6.28898 12.6666 6.11944 12.6666 5.94266C12.6666 5.76589 12.5963 5.59635 12.4714 5.47133Z"
              fill="#626466"
            />
          </svg>
        </span>
      </div>
    </div>
  </div>
</template>

<script>
import CustomButton from './components/CustomButton.vue';
import CustomInput from './components/CustomInput.vue';
import ListItem from './components/ListItem.vue';
export default {
  components: {
    CustomInput,
    CustomButton,
    ListItem,
  },

  data() {
    return {
      data: [
        {
          name: 'Americano',
          image: 'https://picsum.photos/48',
          status: 'green',
          date: null,
        },
        {
          name: 'Espresso',
          image: 'https://picsum.photos/49',
          status: 'yellow',
          date: null,
        },
        {
          name: 'Mocha',
          image: '',
          status: 'green',
          date: null,
        },
        {
          name: 'White Mocha',
          image: '',
          status: 'yellow',
          date: 704305433,
        },
        {
          name: 'Latte',
          image: 'https://picsum.photos/12',
          status: 'green',
          date: 1666715033,
        },
        {
          name: 'Cappucino',
          image: 'https://picsum.photos/33',
          status: 'green',
          date: null,
        },
        {
          name: 'Walking with Giants',
          image: 'https://picsum.photos/64',
          status: 'green',
          date: null,
        },
        {
          name: 'Turbinator 2',
          image: 'https://picsum.photos/87',
          status: 'red',
          date: null,
        },
        {
          name: 'Super Cali Fragilistic Expialidocious',
          image: '',
          status: 'red',
          date: 704305433,
        },
        {
          name: 'Baseball Hat',
          image: 'https://picsum.photos/78',
          status: 'green',
          date: null,
        },
        {
          name: 'Americano',
          image: 'https://picsum.photos/46',
          status: 'green',
          date: null,
        },
        {
          name: 'Espresso',
          image: 'https://picsum.photos/99',
          status: 'yellow',
          date: null,
        },
        {
          name: 'Mocha',
          image: '',
          status: 'green',
          date: null,
        },
        {
          name: 'White Mocha',
          image: '',
          status: 'yellow',
          date: 704305433,
        },
        {
          name: 'Latte',
          image: 'https://picsum.photos/43',
          status: 'green',
          date: 1666715033,
        },
        {
          name: 'Cappucino',
          image: 'https://picsum.photos/75',
          status: 'green',
          date: null,
        },
        {
          name: 'Walking with Giants',
          image: 'https://picsum.photos/97',
          status: 'green',
          date: null,
        },
        {
          name: 'Turbinator 2',
          image: 'https://picsum.photos/30',
          status: 'red',
          date: null,
        },
        {
          name: 'Super Cali Fragilistic Expialidocious',
          image: '',
          status: 'red',
          date: 704305433,
        },
        {
          name: 'Baseball Hat',
          image: 'https://picsum.photos/74',
          status: 'green',
          date: null,
        },
      ],
    };
  },
};
</script>
