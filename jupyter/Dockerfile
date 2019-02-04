FROM jupyter/minimal-notebook:02d387b31c18

ADD ./requirements.txt /tmp/requirements.txt

RUN pip install -r /tmp/requirements.txt 

ADD ./notebooks $HOME/ltibootcamp

USER root
RUN fix-permissions $HOME/ltibootcamp
USER $NB_UID
