# vue-2.4.1-test

This is an issue report.

https://github.com/vuejs/vue/issues/6146

This bug was fixed in vue 2.4.2:

https://github.com/vuejs/vue/commit/082fc3967db4d3290e901a38504dcd9bb698e561


> Vue 2.3.4 & 2.4.1 has different behavior in pre tag compilation


## Steps to Reproduce


1. demo in 2.3.4

```bash
# install vue2.3.4 and vue-template-compiler 2.3.4
npm install

npm run dev
```

Which works well.


![2.3.4](https://raw.githubusercontent.com/clancyz/vue-2.4.1-test/master/2.3.4.jpg)
![2.3.4](https://raw.githubusercontent.com/clancyz/vue-2.4.1-test/master/2.3.4html.png)


2. demo in 2.4.1

```bash
# install vue2.3.4 and vue-template-compiler 2.3.4
npm i vue@2.4.1 vue-template-compiler@2.4.1

npm run dev
```
The demo code is **inline** now:


![2.4.1](https://raw.githubusercontent.com/clancyz/vue-2.4.1-test/master/2.4.1.jpg)
![2.4.1](https://raw.githubusercontent.com/clancyz/vue-2.4.1-test/master/2.4.1html.png)


### By compare two html contents it seems `\n` has removed in 2.4.1.

