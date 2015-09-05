FROM mhart/alpine-node:0.10

#compass
RUN apk add --update build-base libffi-dev ruby ruby-dev git \
    && gem install sass compass --no-ri --no-rdoc \
    && apk del build-base libffi-dev ruby-dev \
    && rm -rf /var/cache/apk/* \
    && npm install -g grunt grunt-cli bower --production

#native libs
#RUN apk-install make gcc g++ python

CMD ["node"]
