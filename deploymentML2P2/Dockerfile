FROM tensorflow/serving

ENV MODEL_BASE_PATH /models
ENV MODEL_NAME customerreview
ENV PORT 8501

COPY model /models

COPY tf_serving_entrypoint.sh /usr/bin/tf_serving_entrypoint.sh
RUN chmod +x /usr/bin/tf_serving_entrypoint.sh
ENTRYPOINT []
CMD ["/usr/bin/tf_serving_entrypoint.sh"]