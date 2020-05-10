# I'll Have The Salad (50)

## Instructions

Bob and Alice love to go to the local farmer's market to get their groceries. You could call them regulars. They know the farmers so well that they've started sharing secret messages with them. Here's one of the messages they wrote to one lettuce farmer.

`vpxoa{eP5o_4_R4mH_pK_1_4421_9952}`

Author: c

## Solution

Let's use Caesar with an offset of 5:

~~~
$ echo "vpxoa{eP5o_4_R4mH_pK_1_4421_9952}" | tr 'A-Za-z' 'F-ZA-Ef-za-e'
auctf{jU5t_4_W4rM_uP_1_4421_9952}
~~~

## Flag
~~~
auctf{jU5t_4_W4rM_uP_1_4421_9952}
~~~
