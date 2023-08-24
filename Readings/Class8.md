## DRY (Don't Repeat Yourself)
DRY is used to reduce redundancy and promote maintainability by having a single, authoritative source of information that can be referenced whenever needed.

## Rule of Three
 It states that two instances of similar code do not require refactoring, but when similar code is used three times, it should be extracted into a new procedure. 
 
 - the last two labs (lab6 and lab7) was about classes that have some common methods and attributes, so I used inheritance from a super class to apply DRY principle.
 - I will determine the repeated code, then I will try to include the repeated code one time only if I can or twice, otherwise I will try to include th erepeated code in a function and refactor my code by calling this function.

 ## Minimum Viable Product (MVP)
 - *Benefits of Releasing an MVP*
 1. gather feedback from real users and customers.
 2. speeds up the development cycle and allows you to get the product to market quickly.
 3. pivot or adjust direction before investing more heavily.
 4. adapt and make improvements based on actual user experiences

 - *Potential Pitfalls of Waiting for Full Maturity*
 1. the product might not align with actual customer needs or preferences.
 2. can result in complex, costly, and time-consuming development that may not align with market demands.
 3. Waiting for maturity might mean missing out on early-stage learning that could shape the product's direction.
 4. Waiting until a product is fully mature before releasing it can lead to lengthy development cycles.