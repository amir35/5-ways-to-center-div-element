5 ways to center div vertically and Horizantally.

1. Flexbox

.right {
    display: flex;
    justify-content: center;
    align-items: center;
}

2. Using absolute positioning and transform

<div class="right">
                <p class="child">
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. <br>
                Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, <br>
                when an unknown printer took a galley of type and scrambled it to make a type <br>
                specimen book. It has survived not only five centuries, but also the leap into <br>
                electronic typesetting, remaining essentially unchanged. It was popularised in <br>
                the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, <br>
                and more recently with desktop publishing software like Aldus PageMaker <br>
                including versions of Lorem Ipsum.
                </p>
            </div>

.right {
    position: relative;
}

.child {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%); /*center both horizontally and vertically */
}


3. Using Grid

.right {
    display: grid;
    place-items: center; /* center both Horizantally and vertically */
}

4. Using table cells and vertical-align

.right {
    display: table-cell;
    text-align: center;
    vertical-align: middle;
}

5.Using position and negative margins

<div class="right">
                <p class="child">
                    Lorem Ipsum is simply dummy text of the printing and typesetting industry. <br>
                Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, <br>
                when an unknown printer took a galley of type and scrambled it to make a type <br>
                specimen book. It has survived not only five centuries, but also the leap into <br>
                electronic typesetting, remaining essentially unchanged. It was popularised in <br>
                the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, <br>
                and more recently with desktop publishing software like Aldus PageMaker <br>
                including versions of Lorem Ipsum.
                </p>
            </div>

.right {
    position: relative;
}

.child {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    margin: -50px 0 0 -50px;
}