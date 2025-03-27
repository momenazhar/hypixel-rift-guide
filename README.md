# Hypixel SkyBlock Rift Guide

`rift_guide.json` contains the API fields of SkyBlock API mapped to their corresponding tasks in the Rift Guide menu.

The structure is as follows:

```ts
type SingleTask = {
    id: string;
    name: string;
    description: string;
    wiki?: string;
};

type GroupTask = {
    name: string;
    description: string;
    tasks: SingleTask[];
};

type Task = SingleTask | GroupTask;
```
