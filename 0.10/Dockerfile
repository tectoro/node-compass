FROM mhart/alpine-node:0.10

#compass
RUN apk add --update build-base libffi-dev ruby ruby-dev \
    && gem install sass compass --no-ri --no-rdoc \
    && apk del build-base libffi-dev ruby-dev \
    && rm -rf /var/cache/apk/*

#native libs
#RUN apk-install make gcc g++ python
RUN npm install -g grunt grunt-cli bower

CMD ["node"]
