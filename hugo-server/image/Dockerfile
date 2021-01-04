ARG SOURCE_IMAGE="klakegg/hugo:0.79.1-ext"
FROM ${SOURCE_IMAGE}

ARG HUGO_SITE="https://github.com/wowchemy/starter-academic.git"
RUN git clone "$HUGO_SITE" /src

CMD [ "server" ]
