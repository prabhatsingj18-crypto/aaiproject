# aaiproject
sd
fsdf
sdaf
asdf
asd
fas
df
asdf
asd
fasdfsdfasf
<h1>digitla marketing</h1>
<p>
  <span id="copyText">Hello World</span>
  <button onclick="copyText()" style="border:none;background:none;cursor:pointer;">📋</button>
</p>

<script>
  function copyText() {
    const text = document.getElementById("copyText").innerText;

    // Modern method (secure context required)
    if (navigator.clipboard && window.isSecureContext) {
      navigator.clipboard.writeText(text).then(() => {
        alert("Copied: " + text);
      });
    } else {
      // Fallback method
      const ta = document.createElement("textarea");
      ta.value = text;
      document.body.appendChild(ta);
      ta.select();
      document.execCommand("copy");
      document.body.removeChild(ta);
      alert("Copied (fallback): " + text);
    }
  }
</script>

