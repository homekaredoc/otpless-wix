# otpless-wix
<script>
    function otpless(otplessUser) {
        const token = otplessUser.token;
        console.log('User Logged In! Token:', token);
        console.log('User Data:', JSON.stringify(otplessUser));

        // Send user data to Wix using postMessage
        window.parent.postMessage(otplessUser, "*");
    }
</script>
