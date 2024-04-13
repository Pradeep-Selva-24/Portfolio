<template>
    <div class="clsContact">
        <div class="clscontent">
            <div class="clsTitle">Contact</div>
            <div class="clsDescription">Feel free to reach out to me for any questions or opportunities!</div>
            <div class="clsFields">
                <div class="clsDescription-Title">Email Me 🚀</div>
                <input placeholder="Your Email" name="from_email" v-model="MailId">
                <input placeholder="Your Name" name="from_name" v-model="Name">
                <input placeholder="Subject" name="subject" v-model="Subject">
                <textarea placeholder="Message" rows="4" name="message" v-model="Message"></textarea>
                <button class="clsButton" @click="sendEmail">Send</button>
                <label class="clsMessage" v-show="IsErrorMessage">{{ErrorMessage}}</label>
            </div>
        </div>
    </div>
</template>

<script>
import $ from 'jquery';
import emailjs from 'emailjs-com';
export default {
    data: function() {
        return {
            MailId:'',
            Name:'',
            Subject:'',
            Message:'',
            ErrorMessage:'Email sent successfully!',
            IsErrorMessage:false
        };
  },
  methods: {
    sendEmail() {
        var Validation = true;
        if(this.MailId == "" || this.Name == "" || this.Subject == "" || this.Message == ""){
            Validation = false;
        }

        if(Validation){
            const templateParams = {
                email_id: this.MailId,
                from_name: this.Name,
                subject: this.Subject,
                message: this.Message
            };

            //emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', templateParams, 'YOUR_USER_ID')
            emailjs.send('service_7ultyzh', 'template_jpdq84w', templateParams, 'Fu0Opgz8rm2y_2YcJ')
            .then(function(response) {
                if(response != null && response.status == 200)
                {
                    $('.clsMessage').html("Email sent successfully!")
                    $('.clsMessage').show()
                }
                else{
                    $('.clsMessage').html("Unable to send email!")
                    $('.clsMessage').show()
                }
                console.log('Success:', response);
            }, function(error) {
                $('.clsMessage').html("Unable to send email!")
                $('.clsMessage').show()
                console.log('Failed:', error);
            });
        }
        else
        {
            $('.clsMessage').html("Fill up all the fields !")
            $('.clsMessage').show()
        }

      
    }
  }
}
</script>