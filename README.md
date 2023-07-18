# Postman_API_Testing_Scripts_And_Validations

### Testing API Response Codes: 

![postman_01](https://github.com/ss-shrishi2000/Postman_API_Testing_Scripts_And_Validations/assets/65821403/dae43cc6-fb02-4ae9-a84c-574f1e785253)


![postman_02](https://github.com/ss-shrishi2000/Postman_API_Testing_Scripts_And_Validations/assets/65821403/77212292-dc2e-41d7-9712-f7f8789fbf51)


### Testing API Headers:

1. There is a lot of information present in the Headers section but our testing should be testing the "Content-Type".
2. Majorily, what does the "Content-Type" section represent Response Format => JSON, XML, HTML, etc. The format can be (let's say): application/json;  which is termed as "mime type". The type of response/data is called mime-type.
3. So, we need to verify if the content type is in JSON Format or not.
4. We can also perform validation on the "Connection" field.
5. We can also perform validation on the "Expires" field.


![postman_03](https://github.com/ss-shrishi2000/Postman_API_Testing_Scripts_And_Validations/assets/65821403/8e9be22e-659f-47c5-84ef-ca05e34bfdbf)


### Testing Cookies:

1. One issue of testing the cookies is that they are prone to change dynamically or their values keep on changing.
2. But there are some cookies whose value won't change each time dynamically. So we can validate those cookies.

3. Assertion => `pm.expect(pm.cookies.has('language')).to.be.true;`
4. Assertion => `pm.expect(pm.cookies.get('language')).to.eql('en-gb');`

### Testing Response times:

1. As the response time can also vary depending upon multiple factors, we try to check if the Response time is under a specified time limit.



![postman_04](https://github.com/ss-shrishi2000/Postman_API_Testing_Scripts_And_Validations/assets/65821403/b114f1c3-fb36-459f-bf53-524dcd3f1385)

   
