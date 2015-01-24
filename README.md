# alphaCA

openssl/keytool self-signed pki repository tool

1. Create your HOSTS file

    cat>HOSTS<<'EOF'
<<<<<<< HEAD
    &#35; jetty jboss tomcat
    type=jks    host=fu1     prefix=
    type=jks    host=fu2     prefix=
    type=jks    host=fu3     prefix=
    &#35; postgres
    type=crt    host=fu1     prefix=pg
    type=crt    host=fu2     prefix=pg
    &#35; dovecot
=======
    # jetty jboss tomcat
    type=jks    host=fu1     prefix=
    type=jks    host=fu2     prefix=
    type=jks    host=fu3     prefix=
    # postgres
    type=crt    host=fu1     prefix=pg
    type=crt    host=fu2     prefix=pg
    # dovecot
>>>>>>> 625a808c04d1f498b237d320a1c481ea025f1b8f
    type=cat    host=fu3     prefix=dc
    EOF

2. Generate all the good stuff

    ./alphaCA.sh

3. Appreciate what happened

    ls

4. Clean up (leaves HOSTS and *.cnf untouched)

    ./alphaCA.sh clean

5. Do not forget your past

    ls

6. Clean up even more

    ./alphaCA.sh distclean

7. Confront the emptiness of the Void

    ls

8. Goto 1.

