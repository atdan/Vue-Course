<script setup>
// import MyComponent from './components/MyComponent.vue'

// import GlobalStyle from './components/GlobalStyle.vue'
// import LocalStyle from './components/LocalStyle.vue'
// import CombinedStyle from './components/CombinedStyle.vue'
// import ModuleStyle from './components/ModuleStyle.vue'

// import MyEvent from './components/MyEvent.vue'

// import MyReactiveComponent from './components/MyReactiveComponent.vue'

// import MyRefComponent from './components/MyRefComponent.vue'

// import ComputedProperties from './components/ComputedProperties.vue'

// import ConditionalRendering from './components/ConditionalRendering.vue'

// import IterationComponent from './components/IterationComponent.vue'

// import FormComponent from './components/FormComponent.vue'

// import StaticPropsComponent from './components/props/StaticPropsComponent.vue'
// import DynamicPropsComponent from './components/props/DynamicPropsComponent.vue'
// const firstName = 'Eustass'
// const lastName = 'Kidd'

// import ChangingPropsValue from './components/props/ChangingPropsValue.vue'
// import PropValidation from './components/props/PropValidation.vue'
// import ComplexProps from './components/props/ComplexProps.vue'
// import CustomValidator from './components/props/CustomValidator.vue'

// import ComponentEventVue from './components/events/ComponentEvent.vue'
// import { ref } from 'vue'
// let count = ref(0)
// const increment = () => count.value++

// import EventValidation from './components/events/EventValidation.vue'
// Creating Methods
// const emit = defineEmits({
//   userInfo: ({ username, email, password }) => {
//     if (!username) {
//       console.log('Please enter your name')
//       return false
//     }
//     if (!email) {
//       console.log('Please enter your email')
//       return false
//     }
//     if (!password) {
//       console.log('Please enter your password')
//       return false
//     } else {
//       return true
//     }
//   }
// })
// const formHandler = (username, email, password) => {
//   emit('userInfo', { username, email, password })
//   console.log('username: ', username)
//   console.log('email: ', email)
//   console.log('password: ', password)
// }

// import SlotComponent from './components/slot/SlotComponent.vue'
// import FallbackContent from './components/slot/FallbackContent.vue'
// import NamedSlot from './components/slot/NamedSlot.vue'
// import DefaultSlot from './components/slot/DefaultSlot.vue'

//---------without provide&inject-----------
// import SchoolComponent from './components/provide&inject/nSchoolComponent.vue'

// const studentName = 'alex'
// const studentAge = 20
// const studentLocation = ['Earth', 'IDK']
//---------------------------------------------

//---------with provide&inject-----------
// import { provide } from 'vue'
// import SchoolComponent from './components/provide&inject/SchoolComponent.vue'
// import PracticeComponent from './components/provide&inject/PracticeComponent.vue'

// provide('studentName', 'Alex')
// provide('studentAge', 20)
// provide('studentLocation', ['Earth', 'IDK'])

//------------------ Practice Provide and Inject Component----------------------
// Using Provide With Array
// provide('friends', ['Alex', 'Jordan', 'HuXn', 'John'])

// // Using Provide With Object
// provide('games', {
//   id: 1,
//   title: 'Epic Adventure Game',
//   genre: ['Action', 'Adventure', 'RPG'],
//   platform: ['PC', 'PlayStation', 'Xbox', 'Nintendo Switch'],
//   releaseDate: '2022-03-15',
//   developer: {
//     name: 'Awesome Game Studios',
//     location: 'San Francisco, CA',
//     teamSize: 50
//   }
// })

// Using Provide With Array Of Objects
// provide('moreGames', [
//   {
//     title: 'Space Explorer',
//     genre: 'Sci-Fi',
//     platform: 'PC',
//     releaseDate: '2023-05-20'
//   },
//   {
//     title: 'Fantasy Quest',
//     genre: 'Fantasy',
//     platform: 'PlayStation',
//     releaseDate: '2023-07-10'
//   },
//   {
//     title: 'Inception',
//     director: 'Christopher Nolan',
//     genre: 'Sci-Fi',
//     releaseDate: '2010-07-16'
//   },
//   {
//     title: 'The Shawshank Redemption',
//     director: 'Frank Darabont',
//     genre: 'Drama',
//     releaseDate: '1994-09-23'
//   }
// ])
//---------------------------------------------

// import LifeCycleHooks from './components/lifecycle/LifeCycleComponent.vue'

// import BasicComponent from './components/watchers/BasicComponent.vue'
// import ReactiveObject from './components/watchers/ReactiveObject.vue'
// import UsingGetterFunction from './components/watchers/UsingGetterFunction.vue'
// import MultipleSources from './components/watchers/MultipleSources.vue'

// import BasicRef from './components/templateRef/BasicRef.vue'
// import FunctionRef from './components/templateRef/FunctionRef.vue'
// import RefComponent from './components/templateRef/RefComponent.vue'

// import ToggleFriends from './components/asyncComponent/ToggleFriends.vue'

// import TodoList from './components/composables/TodoList.vue'
// import CounterComponent from './components/composables/CounterComponent.vue'

// import MyCDComponent from './components/customDirective/MyCDComponent.vue'
import MainComponent from './components/dynamicComponent/MainComponent.vue'
</script>

<template>
  <!-- <MyComponent /> -->

  <!-- <GlobalStyle />
  <LocalStyle />
  <CombinedStyle />
  <ModuleStyle /> -->

  <!-- <MyEvent /> -->

  <!-- <MyReactiveComponent /> -->

  <!-- <MyRefComponent /> -->

  <!-- <ComputedProperties /> -->

  <!-- <ConditionalRendering /> -->

  <!-- <IterationComponent /> -->

  <!-- <FormComponent /> -->

  <!-- <StaticPropsComponent name="Griffon" /> -->
  <!-- <DynamicPropsComponent :firstName="firstName" :lastName="lastName" /> -->
  <!-- <ChangingPropsValue :myFavNumber="9" /> -->
  <!-- <PropValidation fullName="James Garner" :age="21" /> -->

  <!-- <ComplexProps
    :friends="['alex', 'john', 'jordan', 'huxn']"
    :userInfo="{ name: 'alex', age: 20, location: ['Earth', 'IDK'] }"
  /> -->

  <!-- <CustomValidator name="Bonk" :age="21" password="impossiblePassword" /> -->

  <!-- <div>
    <h1>Count: {{ count }}</h1>
    <ComponentEventVue @incrementCount="count++" />
    <ComponentEventVue @incrementCount="increment" />
  </div> -->

  <!-- <EventValidation @userInfo="formHandler" /> -->

  <!-- <SlotComponent>
    <h1>Content 1</h1>
    <h2>Content 2</h2>
  </SlotComponent> -->

  <!-- We didn't specify any content in this component -->
  <!-- <FallbackContent> </FallbackContent>
  <FallbackContent>
    <p>Fallback will not work because I'm providing content inside the component</p>
  </FallbackContent> -->

  <!-- <NamedSlot>
    <template v-slot:one>
      <h1>This content will go to slot "one"</h1>
    </template> -->

  <!-- Alternative way -->
  <!-- <template #two>
      <h1>This content will go to slot "two"</h1>
    </template>
  </NamedSlot> -->

  <!-- <DefaultSlot>
    <template #default>
      <h1>This is some random default content</h1>
    </template>
  </DefaultSlot> -->

  <!-- <SchoolComponent
    :studentName="studentName"
    :studentAge="studentAge"
    :studentLocation="studentLocation"
  /> -->

  <!-- <PracticeComponent /> -->

  <!-- <LifeCycleHooks /> -->

  <!-- <BasicComponent /> -->
  <!-- <ReactiveObject /> -->
  <!-- <UsingGetterFunction /> -->
  <!-- <MultipleSources /> -->

  <!-- <BasicRef /> -->
  <!-- <FunctionRef /> -->
  <!-- <RefComponent /> -->

  <!-- <ToggleFriends /> -->

  <!-- <CounterComponent />
  <TodoList /> -->

  <!-- <MyCDComponent /> -->

  <MainComponent />
</template>

<style scoped></style>
