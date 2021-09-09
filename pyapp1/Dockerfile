FROM python:3-alpine
RUN adduser -D pipuser
USER pipuser
WORKDIR /home/pipuser
COPY --chown=pipuser:pipuser . .
ENV PATH="/home/pipuser/.local/bin:${PATH}"
RUN pip install --user -qr requirements.txt
EXPOSE 8001
CMD ["python3", "./server.py"]
