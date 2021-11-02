FROM python:3.8.12-alpine3.14
RUN adduser -D pipuser
USER pipuser
WORKDIR /home/pipuser
COPY --chown=pipuser:pipuser . .
ENV PATH="/home/pipuser/.local/bin:${PATH}"
RUN pip install --user -qr requirements.txt
EXPOSE 8001
CMD ["python3", "./server.py"]
