Why search for the flag when I can make a bookmarklet to print it for me?
Browse here, and find the flag!

An vao link ta duoc 

![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/ffc9b2f0-5c6e-420e-8537-d424a445447d)

        javascript:(function() {
            var encryptedFlag = "àÒÆÞ¦È¬ëÙ£ÖÓÚåÛÑ¢ÕÓ¨ÍÕÄ¦í";
            var key = "picoctf";
            var decryptedFlag = "";
            for (var i = 0; i < encryptedFlag.length; i++) {
                decryptedFlag += String.fromCharCode((encryptedFlag.charCodeAt(i) - key.charCodeAt(i % key.length) + 256) % 256);
            }
            alert(decryptedFlag);
        })();

  Vao compiler online javascript

  (https://onecompiler.com/javascript/42b58q43m)

  ![image](https://github.com/yeuubonn2k4/Pico/assets/161863346/aa0a3123-8323-420d-aabd-83477517d5c8)

  ta duoc flag 

  picoCTF{p@g3_turn3r_18d2fa20}
