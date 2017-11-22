# CSS Naming Methodologies

This repo gives an overview of multiple CSS naming methodologies and their pros and cons.

## BEM (Block Element Modifier)

**Information**

- http://getbem.com/
- https://css-tricks.com/bem-101/
- https://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/
- https://www.smashingmagazine.com/2016/06/battling-bem-extended-edition-common-problems-and-how-to-avoid-them/

**Pros**

- Component based
- Very flexible, suitable for small and big projects
- Big community so most problems/questions you will face are already 'solved' by others
- No more specificity issues
- Every element has it's own class so you won't have to use descendant selectors anymore. This will improve CSS efficiency
- Can be easily checked by a linter

**Cons**

- Syntax doesn’t look very sexy
- Classnames might get long but this can be solved easily by using the tips out of the following [article](https://www.smashingmagazine.com/2016/06/battling-bem-extended-edition-common-problems-and-how-to-avoid-them/)

## OOCSS (Object Oriented CSS)

**Information**

- https://www.smashingmagazine.com/2011/12/an-introduction-to-object-oriented-css-oocss/
- http://oocss.org/
- http://thesassway.com/intermediate/using-object-oriented-css-with-sass

**Pros**

- Less repeating styles so smaller file size
- Can be used really well in combination with SASS
- CSS styles are modular blocks of code so they can be reused really easy

**Cons**

- Cluttered HTML markup
- Not suitable for small projects
- You probably need to update HTML when updating styles so this makes it really tough to maintain projects.

## SMACSS (Scalable and Modular Architecture for CSS)

**Information**

- https://smacss.com/
- https://www.sitepoint.com/bem-smacss-advice-from-developers/ (also a part about BEM)
- https://bramsmulders.com/blog/how-i-improved-my-workflow-with-smacss-sass/
- https://webuild.envato.com/blog/how-to-scale-and-maintain-legacy-css-with-sass-and-smacss/

**Pros**

- When writing new CSS you probably know where to put it
- Can be used in combination with other methodologies like BEM

**Cons**

- Not really suitable for smaller projects
- Theme might not be needed for all projects
- When using SMACSS without another naming methodology you’re probably still gonna use descendant selectors (which is bad practice and generally should be avoided)

## ACSS (Atomic CSS)

**Information**

- https://acss.io/
- http://www.creativebloq.com/css3/atomic-css-11619006
- https://css-tricks.com/lets-define-exactly-atomic-css/

**Pros**

- Change styles without changing CSS
- Works well with frameworks like React or Angular. Personally I would rather go for something like [Styled Components](https://www.styled-components.com/) but to each his own
- Ultra reusable, never have to duplicate a single line of styling again

**Cons**

- Your HTML elements will have a lot of classes so they will be cluttered
- You need JavaScript to set ACSS up
- CSS doesn’t describe context of components

## Also interesting to check out

**ITCSS (Inverted Triangle CSS)**

- https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/
- http://www.creativebloq.com/web-design/manage-large-css-projects-itcss-101517528
- https://medium.com/@pistenprinz/css-at-trivago-part-1-structure-and-itcss-52f63ed557ca

**CSS namespacing**

- https://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces/
- https://zellwk.com/blog/css-architecture-2/
