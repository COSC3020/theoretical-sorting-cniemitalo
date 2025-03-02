# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

### My Answer

I would verify this claim by evalutating the code using two different sets of different sizes, ensuring that the time complexity increases linearly as the research claims it should. I would then repeat these tests for every different variation of the sets, insuring it covers the bases of sorted, reverse sorted, and everything in between. The timing for both sets of different sizes, no matter the sorting pattern, would need to increase linearly every time in order for the research to be correct about about their program being of $\Theta(n)$. 

As stated in the sorting lecture, the complexity of a comparision based sorting algorithm is $\Omega(nlogn)$, so therefore the algorithm cannot have a runtime complexity of $\Theta(n)$, as it is simply not possible for a comparision based sorting algorithm, giving the minimum number of elements it is required to compare. 
