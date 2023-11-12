FROM tensorflow/tensorflow:latest-gpu
WORKDIR /tf-demer
COPY requirements.txt /tf-demer/requirements.txt
RUN pip install --upgrade pip
RUN pip install --upgrade -r /tf-demer/requirements.txt
RUN pip install ipykernel -U --user --force-reinstall
EXPOSE 8888
ENTRYPOINT ["jupyter", "lab","--ip=0.0.0.0","--allow-root","--no-browser"]