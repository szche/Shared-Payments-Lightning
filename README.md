# Multi-Payer payments using the Lightning Network


## The problem
Let's say you and a random person you've just met wants to buy something online (using the Lightning Network) and split the bill. The merchant hands you a single invoice since he doesn't want to deal with the hassle of generating multiple small invoices and tracking them. Just like in real life payments, it's on you to make the split before/after the invoice is fulfilled. 
The problem arises when you can't trust your newly met friend enought to front him the money and let him pay the invoice in full. The lack of trust goes both ways and your friend is not willing to pay first and get your part from you later.

Consider another situation, you want to donate to your favourite non-profit organization. Upon doing some research, you find that another person promises to match all donations made towards that organization. Now from the previous example we've learnd that you don't really trust some random people met on the internet to keep their word and you want a confirmation of the matched donation. The other party assures you of his good intetions and tells you "Don't worry, I will give you a screenshot of my matched donation". **What if his word is not enough for you?**
Similarly, what is the person that promises to match donations doesn't trust your screenshot as a proof of donating. After all you could've donated $1 and later photoshopped it to be $1000.

**With the current Lightning implementation it is not possible to fulfill one invoice with many payments. So how to solve this problem without using trusted third parties?**

