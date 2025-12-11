This is the testing plan for my Silver Origins project. It incorporates the user stories and boundary test data from before.

**User Stories and Acceptance Criteria**

User Story 1: As a fan of the characters Silver and Blaze, I want their origin stories to make as much sense as possible, so I can understand them even better.  
\- Acceptance Criterion 1: The game will progress throughout the storyline in a correct order.  
\- Acceptance Criterion 2: The game shows an accurate and interesting origin story for both characters.

User Story 2: As an artist, I want the game to embrace colorful graphics and sensational scenery, so it can inspire more of my artwork.  
\- Acceptance Criterion 1: The game will include cool visuals and rendering, especially for fights and other dramatic scenes  
\- Acceptance Criterion 2: The game makes the user feel like they are there in the moment for climatic scenes in the game.

User Story 3: As a storymode-game enthusiast, I want this game to be worthwhile, with many different stages.  
\- Acceptance Criterion 1: The game will have enough stages to keep the average player in the story for 1-2 months, depending on how much they play on an average basis.  
\- Acceptance Criterion 2: The game provides a worthwhile experience for all users.

**Boundary and Edge Testing**

Boundary / Edge 1: health  
    \- Test Case 1: To make sure there is a maximum health  
        a) Upper Boundary: 100  
        b) Testing data used: Player has 120 hp but shouldn’t go over 100  
        c) Expected Result / Behavior: Player can only have 100 hp at most  
        d) Automation Candidate: yes

    \- Test Case 2: To see if negative hp is even possible  
        a) Lower Boundary: 0  
        b) Testing data used: Player at \-5 hp and still alive \- shouldn't be possible  
        c) Expected Result / Behavior: Player can’t go below 0 hp  
        d) Automation Candidate: yes

Boundary / Edge 2: timer  
    \- Test Case 1:  
        a) Upper Boundary: x \> 0  
        b) Testing data used: Player still in-play even when timer hit 0  
        c) Expected Result / Behavior: Game level ends  
        d) Automation Candidate: yes

    \- Test Case 2: To see if a game level ends when the timer reaches 0  
        a) Lower Boundary: 0  
        b) Testing data used: Timer is at \-15 when level should be over at 0  
        c) Expected Result / Behavior: Game over when timer reaches 0  
        d) Automation Candidate: yes

Boundary / Edge 3: inventory  
    \- Test Case 1: To make sure player can have at least 4 items in inventory  
        a) Upper Boundary: 4  
        b) Testing data used: Player can’t pick up more than 2  
        c) Expected Result / Behavior: Player should be able to pick up 2 more items  
        d) Automation Candidate: yes

    \- Test Case 2: To see if items can be picked up when 0 spaces are left  
        a) Lower Boundary: x \> 4  
        b) Testing data used: Player picks up a fifth item when there are only 4 spaces  
        c) Expected Result / Behavior: Player can’t pick up fifth item  
        d) Automation Candidate: yes