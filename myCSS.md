## CSS Key Elements

- Selector
- Box Model - Margin /  Border / Padding
- Position
    - static / relative / absolute / fixed
- Display
    - BASIC : inline / block / inline-block / none
    - RWD : grid / flex
- Float
    - let text could around the specific element
- RWD
    - Media Queries
        
        ```css
        /* Example */
        @media (min-width: 600px) and (max-width: 900px) {
        	/* css for the screen > 600px and screen < 900px */
        }
        ```
        
    - Flexbox (for 1D layout design, e.g., row elements)
        
        ```css
        /* 
        	Example, 
        	Online Document: https://css-tricks.com/snippets/css/a-guide-to-flexbox/ 
        	Online Practices: https://appbrewery.github.io/flexboxfroggy/	
        */
        .flexBox {
        	display: flex;
        	flex-drirection: row (default) / column;
        	flex-basis: 100px; 
        	flex-wrap: nowrap (default) / wrap;
        	justify-content: flex-start / flex-end / center / space-between / space-around / space-evenly;
          align-item: flex-start / flex-end;	
        }
        
        /* 
        	Example, 
        	Hint: content width < width < flex-basis < min-width/max-width
        */
        .flexItem {
        	flex-grow: 1;
        	flex-shrink: 1;
        	flex-basis: 50px;	
        	/* === flex: 1 1 50px; */
        }
        ```
        
    - Grid (for 2D layout design)
        
        ```css
        /* 
        	Example,
        	Online Practices: https://appbrewery.github.io/gridgarden/ 
        */
        .container {
        	display: grid;
        	grid-template-columns: 1fr 2fr;
        	grid-template-rows: 1fr 1fr;
        	/* === 	grid-template-rows: repeat(times, width); */
        	grid-template-rows: auto;
        	
        	/* grid order control */
        	grid-column-start: 1
        	grid-column-end: 2
        	grid-row-start: 3
        	grid-row-end: 4
        	/* === grid-area: 3, 1, 4, 2 */
        	
        	/* grid cell merge */
        	grid-row: span 2
        	
        	gap: 10px;
        }
        ```
