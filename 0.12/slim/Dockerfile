FROM mhart/alpine-node:0.12

#compass
RUN apk add --update build-base libffi-dev ruby ruby-dev \
    && gem install sass compass --no-ri --no-rdoc \
    && apk del build-base libffi-dev ruby-dev \
    && rm -rf /var/cache/apk/*

CMD ["node"]
