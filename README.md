<!DOCTYPE html>
<style>
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    a {
        color: #000;
    }

    button {
        border-style: none;
        margin: 10px;
        padding: 10px;
    }

    button:hover {
        background-color: #888;
    }
</style>
<h1>
    <a href="https://drive.google.com/file/d/1ue9PhXliDH5QUBB7U40OozEbHkETIQy8/view?usp=drive_link">Download executable</a><br>
    <a href="https://drive.google.com/file/d/1jGftxJlCTQS4oJf_7D0VNAyh1aRVzR43/view?usp=sharing">Download 1.3 pck</a><br>
</h1>
<div id="instructions">
    <div id="hidden">
        <button class="tab-button" onclick="toggleInstructions()">Show instructions</button>
    </div>
    <div id="shown">
        <button class="tab-button" onclick="toggleInstructions()">Hide instructions</button>
        <p>
            <ol>
                <li>If you don't have the executable, download it (You only need one, even across versions)</li>
                <li>Download the latest pck</li>
                <li>Make sure the pck and the executable are in the same folder (that folder can just be downloads if you want)</li>
                <li>Double click "Out at dark.exe" to play</li>
            </ol>
        </p>    
    </div>
</div>
<h4>Version 1.0 changes</h4>
<ul>
    <strong><li>Game created</li></strong>
    <a href="https://drive.google.com/file/d/1bKXWH9OVq3Y-RfprrIsUtizBXtxrnRpB/view?usp=sharing">Download 1.0 pck</a>
</ul>
<h4>Version 1.1 changes</h4>
<ul>
    <li>Made level 3 jump easier</li>
    <strong><li>Made level 5 ledges walkable</li></strong>
    <li>Made level 9 gap shorter</li>
    <li>Fixed box dissapearing glitch</li>
    <li>Made instruction labels more clear</li>
    <a href="https://drive.google.com/file/d/1nqdf3hBjM1UHzOT_rHLa3p5UqeX5Ghu9/view?usp=sharing">Download 1.1 pck</a>
</ul>
<h4>Version 1.2 changes</h4>
<ul>
    <strong><li>Added level 10</li></strong>
    <li>Added night sky</li>
    <li>Fixed box hopping (mostly)</li>
    <li>Fixed reset surfing</li>
    <li>Fixed throwing (throw with Q)</li>
    <li>Changed some instruction labels</li>
    <a href="https://drive.google.com/file/d/1BE5ijKNoTq7D1vL6u8L_eTRtiB4d4b8Z/view?usp=sharing">Download 1.2 pck</a>
</ul>
<h4>Version 1.3 changes</h4>
<ul>
    <strong><li>Added Level 11</li></strong>
    <li>Made level 5 significantly easier (Added a lot of run-ups)</li>
    <li>Fixed the level 7 shortcut</li>
    <li>Made it so that you cannot jump over the blocks in level 8</li>
    <li>Added a few instruction labels</li>
    <li>Added a killzone</li>
    <a href="https://drive.google.com/file/d/1jGftxJlCTQS4oJf_7D0VNAyh1aRVzR43/view?usp=sharing">Download 1.3 pck</a>
</ul>
<h4>Version 1.4 changes (unreleased)</h4>
<ul>
    <strong><li>Added Level 12</li></strong>
    <li>Fixed another box dissapearing glitch</li>
    <li>Removed killzone (It was causing box dissapearing glitch)</li>
</ul>
<script>
    var hidden = true;
    var hiddenPane = document.getElementById("hidden");
    var shownPane = document.getElementById("shown");
    hiddenPane.style.display = 'block';
    shownPane.style.display = 'none';
    function toggleInstructions() {
        if (hidden == true) {
            hiddenPane.style.display = 'none';
            shownPane.style.display = 'block';
            hidden = false;
        }
        else {
            hiddenPane.style.display = 'block';
            shownPane.style.display = 'none';
            hidden = true;
        }
    }
    function changeTab(tabId) {
        var tabPanes = document.getElementsByClassName("tab-pane");
        for (var i = 0; i < tabPanes.length; i++) {
            tabPanes[i].style.display = 'none';
        }
        var tabPane = document.getElementById(tabId);
        tabPane.style.display = "block";

    }
    changeTab('hide')
</script>
<p></p>
