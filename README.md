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

I would verify this claim by evalutating the code using different sets of different sizes, ensuring that the time complexity increases linearly as the researcher claims it should. I would then repeat these tests for every different variation of the sets, insuring the inputs cover the bases of sorted, reverse sorted, empty, and everything in between. I would probably repeat this process for multiple different sets, including duplicate elements, to ensure the algorithm doesn't depend on a certain input. The timing for the different sizes, no matter the sorting pattern, would need to have a linear runtime comparision every time in order for the research to be correct about about their program being of $\Theta(n)$. 

As stated in the sorting lecture, the complexity of a comparision based sorting algorithm is $\Omega(nlogn)$, so therefore the algorithm cannot have a runtime complexity of $\Theta(n)$, as it is simply not possible for a comparision based sorting algorithm, given that sorting n elements takes nlogn comparisions. 

## Sources and Plagiarism 

Class sorting lecture slides 

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
