<script>
    export let year;
</script>

<footer>
    <div class="footerContents">
        <div>
            <h3>Services</h3>
            <p class="firstP" id="linkP">Branding</p>
            <p id="linkP">Design</p>
            <p id="linkP">Marketing</p>
            <p id="linkP">Advertisement</p>
        </div>
        <div>
            <h3>Company</h3>
            <p class="firstP" id="linkP">About us</p>
            <p id="linkP">Contact us</p>
            <p id="linkP">Jobs</p>
            <p id="linkP">Press kit</p>
        </div>
        <div>
            <h3>Legal</h3>
            <p class="firstP" id="linkP">Terms of use</p>
            <p id="linkP">Privacy policy</p>
            <p id="linkP">Cookie policy</p>
        </div>
    </div>

    <p class="bottomP">Maja Birch Sørensen © {year} </p>
</footer>

<style>
    footer {
        background-color:#3E4450;
        padding-top: 25px;
        border-radius: 5px;
    }
    .firstP {
        margin-top: 0;
    }
    .footerContents {
        margin-top: 20px;
        
    }
     @media only screen and (min-width: 800px) {
        .footerContents {
            column-count: 3;
            display: flex;
            justify-content: space-evenly;
        }
    }
    p {
        font-size: small;
        color: #e7e7e7;
        font-weight: 600;
        overflow: hidden;
    }
    #linkP {
        overflow: hidden;
        border-bottom: 1.5px solid #3E4450;
        width: fit-content;
        padding-bottom: 3px;
    }
    #linkP:hover {
        cursor: pointer;
        border-bottom: 1.5px solid #D3D4D6;
    }
    .bottomP {
        font-size: x-small;
        text-align: center;
        margin: 0;
        padding: 30px;
        
    }
    h3 {
        color: #A6A8AE;
    }
</style>